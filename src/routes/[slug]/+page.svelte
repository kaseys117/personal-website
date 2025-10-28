<script lang="ts">
	import type { PageProps } from './$types';
	import { page } from '$app/state';
	import portfolio from './portfolio.json';
	let { data }: PageProps = $props();

	let { slug } = page.params;

	let project = fetchProject(slug);

	function fetchProject(slug: string) {
		for (const project of portfolio) {
			if (slug === project.slug) return project;
		}
	}
</script>

<h1>{project!.title}</h1>

<div class="mx-15 mt-5">

<div class="tools">
    {#each project!.tools as tool}
        <span>
            {tool}
        </span>
    {/each}
</div>

<p class="details">
    {project!.details}
</p>

<b class="title">Lessons Learned</b>

<p class="lessons-learned">{project!.lessons_learned}</p>

</div>

<style>

    .tools{
    display: flex;
    gap: .5rem;
    margin-bottom: 2rem;
    }

    .details{
    width: 45ch;
    }

    span {
    padding: .25rem .5rem;
    border: 1px solid white;
    border-radius: 15px;
    background-color: #e5e2f4;
    color: #454863;
    font-size: 13px;
    font-weight: bold;
    }
</style>
