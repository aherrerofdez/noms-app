<script>
	import Layout from './__layout.svelte'

	let menu = 4;

	let bundles = ['/content/bundles/blue-bundle.jpg',
		           '/content/bundles/green-bundle.jpg',
		           '/content/bundles/red-bundle.jpg']
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

<Layout menu={menu} />

<div class="slider">
    {#each bundles as bundle}
	    <section>
            <img src={bundle} alt="Grocery shopping list for the set of recipes displayed">
        </section>
    {/each}
</div>
