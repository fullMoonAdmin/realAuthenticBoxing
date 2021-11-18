<script>
    import Nav from "../components/nav.svelte";
    import Footer from "../components/footer.svelte";
</script>

<Nav />

<slot />

<Footer />

<style>
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
</style>
