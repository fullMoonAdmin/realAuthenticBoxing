<script>
    import Contact from "../components/contact.svelte";
    import FighterCards from "../components/fighterCards.svelte";
</script>

<div class="flex-area">
    <FighterCards />
    <Contact />
</div>

<style>
    .flex-area {
        display: flex;
        flex-wrap: wrap;
        flex-direction: column;
        align-items: center;
        margin-top: 25px;
        margin-bottom: 45px;
    }
</style>
