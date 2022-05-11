<script>
    import Nav from "../components/nav.svelte";
    import Footer from "../components/footer.svelte";
</script>

<Nav />

<slot />

<Footer />

<style>
    @import url("https://fonts.googleapis.com/css2?family=Alfa+Slab+One&display=swap");
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
</style>
