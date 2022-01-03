<script>
    /*var recipes_path = ['/content/recipes/caesar-salad-v.jpg',
                        '/content/recipes/caesar-salad.jpg',
                        '/content/bundles/green-bundle.jpg',
                        '/content/bundles/red-bundle.jpg']*/
    export let recipes_path;

</script>

<style>
    div {
        margin-top: 20px;
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
    {#each recipes_path as recipe}
	    <section>
            <img src={recipe} alt="noms recipe format">
        </section>
    {/each}
</div>