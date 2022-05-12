<script>
    import AwardsGallary from "../components/awardsGallary.svelte";
    import Contact from "../components/contact.svelte";
    import FighterCards from "../components/fighterCards.svelte";
</script>

<div class="flex-area">
    <h1>Awards</h1>
    <div id="gallary-container">
        <AwardsGallary />
    </div>
    <h1>Our Boxers</h1>
    <FighterCards />
    <Contact />
</div>

<style>
    h1 {
        font-family: "Alfa Slab One", cursive;
        font-size: 65px;
        margin: 20px;
    }
    .flex-area {
        display: flex;
        flex-wrap: wrap;
        flex-direction: column;
        align-items: center;
        margin-top: 25px;
        margin-bottom: 45px;
    }
    #gallary-container {
        max-width: 70rem;
        margin: 1rem;
    }
</style>
