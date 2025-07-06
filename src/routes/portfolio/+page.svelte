<script lang="ts">
	import type { PageData } from './$types';

	let { data }: { data: PageData } = $props();
</script>

<h1>Portfolio</h1>

<p class="text-center" style="color: #454863;">
	A selection of projects showcasing my work in cybersecurity and other related work.
</p>

<div class="main">
	<div class="project">
		<h2 class="projecttitle">Blank - TBD</h2>

		<img src="P3.png" style="width: 250px;border-radius: 1rem;" />

		Blank - TBD

		<!-- <img src="Wireshark.png" style="width: 25px;"><br> -->

		<a class="button"> View Project </a>
	</div>

	<div class="project">
		<h2 class="projecttitle">Blank - TBD</h2>

		<img src="P3.png" style="width: 250px;border-radius: 1rem;" />

		Blank - TBD

		<!-- <img src="Wireshark.png" style="width: 25px;"><br> -->

		<a class="button"> View Project </a>
	</div>

	<div class="project">
		<h2 class="projecttitle">IOT - Baby Monitor Security</h2>

		<img src="P3-1.png" style="width: 250px;border-radius: 1rem;" />

		A hands-on project aimed at evaluating the network security of low-cost baby monitors purchased
		from Amazon.

		<!-- <img src="Wireshark.png" style="width: 25px;"><br> -->

		<a class="button"> View Project </a>
	</div>

	<div class="project">
		<h2 class="projecttitle">Wellmo - A Wellness App</h2>

		<img src="P4.png" style="width: 250px;border-radius: 1rem;" />

		A software engineering project aimed at finding the best software development life cycle for an
		app of our choosing.

		<a class="button"> View Project </a>
	</div>

	<div class="project">
		<h2 class="projecttitle">RainCheck - A Weather App</h2>

		<img src="P5-1.png" style="width: 250px;border-radius: 1rem;" />

		An app created with a focus on human-computer interaction. What matters is how UI friendly it is
		for the users.

		<a class="button"> View Project </a>
	</div>

	<div class="project">
		<h2 class="projecttitle">Office Statistics Dashboard</h2>

		<img src="P6.png" style="width: 250px;border-radius: 1rem;" />

		A visual of the office traffic we receive throughout the year. Data ranges from basic counts to
		average student GPA.

		<a class="button"> View Project </a>
	</div>

	<div class="project">
		<h2 class="projecttitle">Process Automation</h2>

		<img src="P7.png" style="width: 250px;border-radius: 1rem;" />

		An automation of office procedures that helped reduce the manual labor while also ensuring and
		maintaining data accuracy.

		<a class="button"> View Project </a>
	</div>
</div>

<style>
	.main {
		display: flex;
		flex-wrap: wrap;
		justify-content: space-between;
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
	}
</style>
