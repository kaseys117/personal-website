<h1>
	<center> Home </center>
</h1>

<p class="text-center" style="color: #454863; margin-bottom: 2rem;">
	 
</p>

<div class="home">
	
	

		<div class="me">
			<img src="Me.png" id="front" width="250px" />
			<img src="Me2.png" id="back" width="250px" />
		</div>

<div class="intro">
		<div class="box1">
			<h2>Why I Built This Site</h2>
			I simply wanted to challenge myself. I had been working with some HTML in my current and previous
			job and I found myself struggling, but I at least understood the gist. One day, I had
			a hit of inspiration and I told myself I would build my own personal website from scratch, meaning
			no templates and no AI. Though I was presented with a lot of challenges and a learning curve, it
			ended up working out. It's safe to say I'm satisfied with my progress and the result of this site
			is evidence of my accomplishment.
		</div>
	
		<div class="box2">
			<h2>What's Next?</h2>
			This website will always be a work in progress as I continue to pursue more projects and certifications.
			The learning is never ending, especially in the field of cybersecurity. Now, it's time to check
			out the rest of my website where you'll find out more about my personal and professional life.
		</div>
	</div>
</div>

<style>

.home{
	display: flex;
	justify-content: center;
	align-items: center;
}

	.intro {
		display: flex;
		flex-direction: column;
		gap: 1rem;
		width: auto;
		align-items: center;
		padding: 0 1rem;
	}


	.box1 {
		font-size: 15px;
		color: #454863;
		padding: 1.5rem 1.5rem 1.5rem 1.5rem;
		border: 1px solid white;
		border-radius: 1rem;
		box-shadow: 0px 4px 10px #d3cedb;
		background-color: #e5e2f4;
		width: 55ch;
	}

	.box2 {
		font-size: 15px;
		color: #454863;
		padding: 1.5rem 1.5rem 1.5rem 1.5rem;
		border: 1px solid white;
		border-radius: 1rem;
		box-shadow: 0px 4px 10px #d3cedb;
		background-color: #e5e2f4;
		width: 55ch;
	}

	h2 {
		font-size: 20px;
		color: #454863;
		font-weight: normal;
		margin-bottom: .5rem;
	}


	.me {
		position:relative;
		width: 300px;
		height: 200px;
		perspective: 1000px;
		transform-style: preserve-3d;
	}

	#front, #back{
		position: absolute;
		top: -3rem;
		left: -3rem;
		transition: transform 1s;
		backface-visibility: hidden;
		outline: 4px solid #d0b7f7;
		outline-offset: 6px;
		margin: 2rem;
		border-radius: 50%;
	}

	#back{
		transform: rotateY(180deg);
	}

	.me:hover #back{
		transform: rotateY(0deg);
	}

	.me:hover #front{
		transform: rotateY(-180deg);
	}

	

	/* img {
		outline: 4px solid #d0b7f7;
		outline-offset: 6px;
		margin: 2rem;
		border-radius: 50%;
		transition: 1s ease-in-out;
	}

	img:hover {
		animation: spin 1s ease-in-out;
	}

	@keyframes spin{
		0%{
			rotate:Y 0deg;
		}
		100%{
			rotate:Y 360deg;
			background-color: red;
			background-size: cover;
			background-repeat: no-repeat;
		}
	} */
	
</style>
