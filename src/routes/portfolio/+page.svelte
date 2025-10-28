<script lang="ts">
	import type { PageData } from './$types';
	import Modal from '$lib/modal.svelte';
	import projects from '$lib/projects.json';

	type ProjectType = {
		title: string;
		description: string;
		tools: string[];
		about: string;
		lessons_learned: string;
		thumbnail: string;
		slug: string;
		img_src: string;
		img_title: string;
	}

	let modal = $state(null);
	let active = $state({});

	let { data }: { data: PageData } = $props();
	function open(project: ProjectType) {
		active = project;
		modal!.showModal();
	}
</script>

<h1>Portfolio</h1>

<p class="text-center" style="color: #454863;">
	A selection of projects showcasing my work in cybersecurity and other related work.
</p>
<Modal bind:modal {...active} />
<div class="main">
	{#each projects as project}

		<div class="project">
			<h2 class="projecttitle">{project.title}</h2>

			<img src={project.img_src} style="width: 250px;border-radius: 1rem;" alt="project thumbnail"/>

			{project.description}

			<button class="button" onclick={() => open(project)}> View Project </button>
		</div>
	{/each}

</div>

<style>
	.main {
		display: flex;
		flex-wrap: wrap;
		justify-content:left;
		gap: 2.5rem;
		margin: 2.5rem;
	}

	.project {
		display: flex;
		flex-flow: column;
		justify-content: space-between;
		gap: 1rem;
		font-size: 16px;
		color: #454863;
		padding: 2rem 1.5rem 1rem 2rem;
		border: 1px solid white;
		border-radius: 1rem;
		box-shadow: 0px 4px 10px #d3cedb;
		background-color: #e5e2f4;
		width: 32ch;
	}

	.projecttitle {
		font-size: 20px;
		color: #454863;
		font-weight: normal;
	}

	.button {
		align-self: center;
		line-height: normal;
		padding: 0.5rem 3rem 0.5rem;
		border-radius: 0.125rem;
		background-color: #462ea3;
		color: white;
		cursor: pointer;
	}
</style>
