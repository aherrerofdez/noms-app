<script>
	let batches = ['/content/series/batch/broccoli-pasta.jpg',
		           '/content/series/batch/chilli-sin-carne.jpg',
		           '/content/series/batch/mushroom-risotto.jpg']
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
    {#each batches as batch}
	    <section>
            <img src={batch} alt="Batch series cooking recipes">
        </section>
    {/each}
</div>