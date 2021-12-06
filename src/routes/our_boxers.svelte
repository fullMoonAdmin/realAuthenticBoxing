<script>
    import Contact from "../components/contact.svelte";
    import FighterCards from "../components/fighterCards.svelte";
</script>

<div class="flex-area">
    <h1>Our Boxers</h1>
    <hr />
    <FighterCards />
    <Contact />
</div>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Alfa+Slab+One&display=swap");
    h1 {
        font-family: "Alfa Slab One", cursive;
        font-size: 45px;
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
    hr {
        margin: 0.5em;
        width: 300px;
        color: gray;
    }
</style>
