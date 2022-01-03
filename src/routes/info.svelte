<script>
    import Layout from './__layout.svelte'

    let menu = 5;
</script>

<style>
    div {
        display: flex;
        align-items: center;
        justify-content: center;
        margin-top: 55px;
    }

    img {
        width: 100%;
    }

</style>

<Layout menu={menu} />

<div>
    <img src="/content/how-to-noms.jpg" alt="Instructions on how to read the recipes">
</div>