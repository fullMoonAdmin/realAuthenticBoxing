<script>
    import Map from "../components/map.svelte";

    import Contact from "../components/contact.svelte";
</script>

<main>
    <div class="flex-container">
        <h1>About Us</h1>
        <img
            src="authenticLogo.svg"
            alt="Authentic Logo"
            width="20px"
            id="logo"
        />
        <p class="sub-title">Authentic Boxing: Professional Boxing Club</p>

        <p class="information">
            Larry Edgar and partner Monty Summers opened the doors to Authentic
            Boxing Club in the Spring of 1999.
        </p>
        <div class="side-by-side">
            <img
                id="coach"
                src="larry.jpeg"
                alt="coach Larry Edgar"
                width="230px"
                marg
            />
            <p id="coach-info">
                Coach Larry Edgar and the Team are striving to become the best
                boxing club in the country. Authentic Boxing Club has the
                reputation of producing Professional boxers, male or female, to
                compete at the highest level of the sport of Boxing. Authentic
                offers professional training and management.
            </p>
        </div>
        <img src="/awards/burnett1.jpeg" alt="" />
        <Map />
        <Contact />
    </div>
</main>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Alfa+Slab+One&display=swap");

    :global(html) {
        background-color: black;
    }
    main {
        margin-top: 25px;
        background-color: black;
        color: gray;
        height: 100vh;
        font-family: "Alfa Slab One", cursive;
        padding-bottom: 25px;
    }
    .flex-container {
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    h1 {
        font-size: 65px;
        text-align: center;
    }
    #logo {
        margin: 2em;
        width: 200px;
    }
    .sub-title {
        margin-top: 1rem;
        text-align: center;
        font-size: large;
        max-width: 350px;
        margin-bottom: 2rem;
    }
    .information {
        max-width: 300px;
        margin-top: 0.5em;
        font-size: small;
        text-align: center;
        text-indent: 1em;
    }
    .side-by-side {
        margin-top: 1rem;
        padding: 1em;
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: space-evenly;
    }
    #coach-info {
        max-width: 300px;
        margin: 1.5em;
        text-indent: 2em;
    }
    #coach {
        width: 305px;
        border-radius: 4px;
    }
</style>
