<script>
    import { onMount } from "svelte";
    import { page } from "$app/stores";
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
    class="flex flex-wrap items-center justify-between p-5 bg-gradient-to-r from-black to-gray-600 sticky top-0 z-50 "
>
    <!-- logo -->
    <a href="/">
        <img
            src="authenticBoxing.jpeg"
            alt="Authentic Logo"
            width="90"
            id="logo"
        />
    </a>
    <!-- hamburger -->
    <div class="flex md:hidden">
        <button id="hamburger">
            <img
                class="toggle block"
                src="hamburger.png"
                width="40"
                height="40"
                alt=""
            />
            <img
                class="toggle hidden"
                src="x.png"
                width="40"
                height="40"
                alt=""
            />
        </button>
    </div>
    <!-- links -->
    <div
        class="toggle hidden md:flex w-full md:w-auto text-right text-bold mt-5 md:mt-0 border-t-2 border-white-900 md:border-none"
    >
        <a
            href="/"
            class="block md:inline-block text-gray-50 hover:text-red-500 px-3 py-3 border-b-2 border-white-900 md:border-none"
            class:active={$page.path === "/"}
        >
            Home
        </a>
        <a
            href="/venue"
            class="block md:inline-block text-gray-50 hover:text-red-500 px-3 py-3 border-b-2 border-white-900 md:border-none"
            class:active={$page.path === "/venue"}
        >
            Venue
        </a>
        <!-- <a
            href="/our_boxers"
            class="block md:inline-block text-gray-50 hover:text-blue-500 px-3 py-3 border-b-2 border-white-900 md:border-none"
            class:active={$page.path === "/our_boxers"}
        >
            Our Boxers
        </a> -->
        <a
            href="/about"
            class="block md:inline-block text-gray-50 hover:text-red-500 px-3 py-3 border-b-2 border-white-900 md:border-none"
            class:active={$page.path === "/about"}
        >
            About
        </a>
    </div>
</nav>

<style>
    nav {
        border-bottom: gray solid 1px;
        margin-top: -16px;
    }
    a {
        font-family: "Alfa Slab One", cursive;
        font-size: 1.5em;
    }
    .active {
        text-decoration: underline;
    }
</style>
