<script lang="ts">
	let {
		modal = $bindable(),
		title,
		tools,
		about,
		lessons_learned,
		img_src,
		img_title,
	} : 
	{
		modal: any;
		title: string;
		description: string;
		tools: string[];
		about: string;
		lessons_learned: string;
		thumbnail: string;
		slug: string;
		img_src: string;
		img_title: string;
	}= $props();
</script>

<dialog bind:this={modal} closedby="any">
	<button onclick={()=>modal.close()}><svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-x"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M18 6l-12 12" /><path d="M6 6l12 12" /></svg>
    </button>

	<h2>
		{title}
	</h2>

	<div class="tools">
		{#each tools as tool}
			<span>
				{tool}
			</span>
		{/each}
	</div>

	<div class="content">
		<div class="text">
			<h3>About</h3>
			<p>{about}</p>
			<h3>Lessons Learned</h3>
			<p>{lessons_learned}</p>
		</div>
		<div class="image">
            <img src={img_src} alt={img_title} />
			<p class="img-label">{img_title}</p>
		</div>
	</div>
</dialog>

<style>
	.content {
		display: grid;
		grid-auto-flow: column;
		grid-template-columns: 50ch minmax(0, auto);
		align-items: center;
		gap: 5rem;
	}

    button{
        margin:1.5rem;
        cursor: pointer;
        position: absolute;
        top:0;
        right:0;
    }

	.image {
		grid-column: 2;
	}

	.text {
		grid-column: 1;
	}

    .tools {
        display: flex;
        gap: .25rem;
        margin: 1.5rem 0;
        span{
            background-color: #e5e2f4;
            border-radius: 1rem;
		    border: 1px solid #ffff;
            padding: 0 .5rem;
            font-size: 13px;
            font-weight: 750;
        }
    }

	dialog {
		font-size: 15px;
		background-color: #e9e4f0;
		padding: 3.5rem 5rem;
		margin: auto 5rem;
		height: 70%;
		border-radius: 1rem;
		border: 1px solid #ffff;
	}

	h2 {
		font-weight: bold;
		font-size: 24px;
		text-align: center;
	}

	h3{
		font-weight: bold;
		font-size: 16px;
		margin-bottom: 0.5rem;
	}

    h3:is(p+h3){
            margin-top: 2.5rem;
        }

    .img-label {
    font-size: 10;
    font-style: italic;
    text-align: center;
    width: 100%;
    margin-top: .5rem;
    }

</style>
