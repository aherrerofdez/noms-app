<script>
	let no_cooks = ['/content/series/no-cook/chickpea-sandwich.jpg',
		            '/content/series/no-cook/peanut-sauce-rolls.jpg',
		            '/content/series/no-cook/tuna-sandwich.jpg']
</script>

<style>

    div {
        margin-top: 56px;
    }

    img {
        width: 100%;
		border-radius: 10px;
		margin-left: 1px;
    }

    .slider {
		scroll-snap-type: x mandatory;	
		display: flex;
		-webkit-overflow-scrolling: touch;
		overflow-x: scroll;
	}

    section {
		min-width: 95vw;
		max-height: 100vh;
		scroll-snap-align: start;
		text-align: center;
		position: relative;
		margin-right: 8px;
	}

</style>

<div class="slider">
    {#each no_cooks as nc}
	    <section>
            <img src={nc} alt="No-cook series cooking recipes">
        </section>
    {/each}
</div>