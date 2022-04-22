<script>
    console.log("lets get it started");
    import Hero from "../components/hero.svelte";
    import Contact from "../components/contact.svelte";
</script>

<svelte:head>
    <title>Strike Night</title>
</svelte:head>

<Hero />
<main>
    <div id="flex-container">
        <Contact />
    </div>
</main>

<style>
    :global(body) {
        background-color: black;
    }
    main {
        background-color: black;
        margin-bottom: 25px;
        color: gray;
    }
    #flex-container {
        display: flex;
        justify-content: center;
    }
</style>
