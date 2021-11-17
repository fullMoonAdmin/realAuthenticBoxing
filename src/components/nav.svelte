<script>
    import { onMount } from "svelte";
    onMount(() => {
        document.getElementById("hamburger").onclick = function toggleMenu() {
            const navToggle = document.getElementsByClassName("toggle");
            for (let i = 0; i < navToggle.length; i++) {
                navToggle.item(i).classList.toggle("hidden");
            }
        };
    });
</script>

<nav
    class="flex flex-wrap items-center justify-between p-5 bg-gradient-to-r from-transparent to-gray-600 sticky top-0 z-50"
>
    <!-- logo -->
    <img src="http://acmelogos.com/images/logo-1.svg" alt="ACME" width="120" />
    <!-- hamburger -->
    <div class="flex md:hidden">
        <button id="hamburger">
            <img
                class="toggle block"
                src="https://img.icons8.com/fluent-systems-regular/2x/menu-squared-2.png"
                width="40"
                height="40"
                alt=""
            />
            <img
                class="toggle hidden"
                src="https://img.icons8.com/fluent-systems-regular/2x/close-window.png"
                width="40"
                height="40"
                alt=""
            />
        </button>
    </div>
    <!-- links -->
    <div
        class="toggle hidden md:flex w-full md:w-auto text-right text-bold mt-5 md:mt-0 border-t-2 border-blue-900 md:border-none"
    >
        <a
            href="#"
            class="block md:inline-block text-gray-50 hover:text-blue-500 px-3 py-3 border-b-2 border-blue-900 md:border-none"
            >Home</a
        >
        <a
            href="#"
            class="block md:inline-block text-gray-50 hover:text-blue-500 px-3 py-3 border-b-2 border-blue-900 md:border-none"
            >Products</a
        >
        <a
            href="#"
            class="block md:inline-block text-gray-50 hover:text-blue-500 px-3 py-3 border-b-2 border-blue-900 md:border-none"
            >Pricing</a
        >
        <a
            href="#"
            class="block md:inline-block text-gray-50 hover:text-blue-500 px-3 py-3 border-b-2 border-blue-900 md:border-none"
            >Contact</a
        >
    </div>
</nav>
