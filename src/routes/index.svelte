<script>
    let inspo = ['/content/inspo/Pasta-Bolognese.png',
		         '/content/inspo/Green-Bruschetta-V.png',
		         '/content/inspo/Caesar-Salad.png',
                 '/content/inspo/Chickpea-Salad.png',
                 '/content/inspo/Taco-Bowl.png']

    let path = "";

    function getRecipe(i) {
        path = '/recipes/' + i.slice(15, -4).toLowerCase();
        path = path.replaceAll(" ", "");
        return path;
    }
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');

    div {
        margin-top: 15px;
    }

    img {
        width: 100%;
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
		max-height: 95vh;
		scroll-snap-align: start;
		text-align: center;
		position: relative;
		margin-right: 8px;
	}

    p {
        font-family: 'Montserrat';
        color: #A2AAAE;
        font-size: 16pt;
        margin: 15px;
    }

</style>

<div class="slider">
    {#each inspo as i}
	    <section>
            <p> {i.slice(15, -4).replaceAll("-", " ")} </p>
            <a href={getRecipe(i)}>
                <img src={i} alt="Daily inspiration recipes">
            </a>
        </section>
    {/each}
</div>