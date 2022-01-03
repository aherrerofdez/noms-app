<script>
    import Layout from './__layout.svelte'

    let menu = 3;
</script>

<style>
    div {
        display: inline-block;
        text-align: center;
        margin-top: 35px;
    }

    a {
        border: none;
        border-radius: 10px;
        padding-bottom: 0;
        background-color: white;
    }

    img {
        width: 80%;
        padding: 0;
        margin-bottom: 35px;
        border: solid #A2AAAE 2px;
        box-shadow: 5px 5px 10px #A2AAAE;
        border-radius: 10px;
    }

</style>

<Layout menu={menu} />

<div>
    <a href="/series/batch">
        <img src="/content/series/batch/batch-series.jpg" alt="Batch series main benefit is convenience">
    </a>
    <a href="/series/no-cook">
        <img src="/content/series/no-cook/nocook-series.jpg" alt="No-cook series main benefit is speed">
    </a>
</div>