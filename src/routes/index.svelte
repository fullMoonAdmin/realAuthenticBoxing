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
    <div class="flex-container">
        <h1>Upcoming Events</h1>
        <img src="may2872022.jpeg" alt="strike night poster" />
    </div>

    <div class="flex-container">
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
        font-family: "Alfa Slab One", cursive;
        font-size: 1.5em;
    }
    h1 {
        font-size: 40px;
        margin-bottom: 1em;
    }
    img {
        width: 60rem;
    }

    .flex-container {
        display: flex;
        justify-content: center;
        flex-direction: column;
        align-items: center;
    }
</style>
