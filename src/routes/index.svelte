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
        
        <img
            src="fightCards/authenticCurrentCard.jpg"
            alt="strike night poster"
            id="fightCard"
        />

        
         
        
        
        <br>
        <br>
        <br>  
        <h3>More Information Coming Soon</h3> 
          
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
        font-size: 2rem;
        margin-top: 1em;
        margin-bottom: 1em;
    }
    h2 {
        font-size: 1.75rem;
        margin-top: 0.5em;
        margin-bottom: 0.5em;
    }
    h3 {
        font-size: 1.25rem;
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
