<script>
    console.log("lets get it started");
    import Hero from "../components/hero.svelte";
    import Contact from "../components/contact.svelte";
</script>

<svelte:head>
    <title>Authentic Boxing</title>
</svelte:head>

<Hero />
<main>
    <div class="flex-container">
        <h1>Upcoming Events</h1>

        
        <p>Strike Night 14 is scheduled for July 30th. Tickets sales and the fight card are comming soon!</p>
        <!--<img
            src="fightCards/authenticCurrentCard.jpeg"
            alt="strike night poster"
            id="fightCard"
        />-->        
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
        margin-top: 1em;
        margin-bottom: 1em;
    }
    img {
        width: 70rem;
    }

    .flex-container {
        display: flex;
        justify-content: center;
        flex-direction: column;
        align-items: center;
    }
    #fightCard {
        border-radius: 4px;
        border: solid 3px silver;
    }
</style>
