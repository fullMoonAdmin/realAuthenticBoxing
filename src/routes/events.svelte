<script>
    import Contact from "../components/contact.svelte";
</script>

<section>
    <h1>Past Events</h1>
    <br />
    <img src="event.jpeg" alt="event poster" />
</section>
<div class="flex-container">
    <Contact />
</div>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Alfa+Slab+One&display=swap");

    :global(html) {
        background-color: black;
    }
    h1 {
        color: gray;
        font-family: "Alfa Slab One", cursive;
        font-size: 65px;
        text-align: center;
    }
    img {
        width: min-content;
        height: min-content;
        margin: auto;
        border-radius: 4px;
    }
    section {
        background-color: black;
        margin-top: 25px;
        height: 100%;
        margin-bottom: 45px;
    }
    br {
        background-color: gray;
        color: gray;
    }
    .flex-container {
        display: flex;
        color: gray;
        justify-content: center;
        margin-top: -80px;
    }
</style>
