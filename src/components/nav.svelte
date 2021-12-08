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
    class="flex flex-wrap items-center justify-between p-5 bg-gradient-to-r from-black to-gray-600 sticky top-0 z-50 "
>
    <!-- logo -->
    <a href="/">
        <img
            src="authenticLogo.svg"
            alt="Authentic Logo"
            width="70"
            id="logo"
        />
    </a>
    <!-- hamburger -->
    <div class="flex md:hidden">
        <button id="hamburger">
            <svg
                xmlns="http://www.w3.org/2000/svg"
                x="0px"
                y="0px"
                width="34"
                height="34"
                class="toggle block"
                viewBox="0 0 172 172"
                style=" fill:#000000;"
                ><g transform="translate(4.988,4.988) scale(0.942,0.942)"
                    ><g
                        fill="none"
                        fill-rule="nonzero"
                        stroke="none"
                        stroke-width="none"
                        stroke-linecap="butt"
                        stroke-linejoin="none"
                        stroke-miterlimit="10"
                        stroke-dasharray=""
                        stroke-dashoffset="0"
                        font-family="none"
                        font-weight="none"
                        font-size="none"
                        text-anchor="none"
                        style="mix-blend-mode: normal"
                        ><g
                            fill="#607d8b"
                            stroke="#cccccc"
                            stroke-width="10"
                            stroke-linejoin="round"
                            ><g
                                ><path
                                    d="M150.5,39.41667v7.16667c0,5.934 -4.816,10.75 -10.75,10.75h-107.5c-5.934,0 -10.75,-4.816 -10.75,-10.75v-7.16667c0,-5.934 4.816,-10.75 10.75,-10.75h107.5c5.934,0 10.75,4.816 10.75,10.75z"
                                /><path
                                    d="M150.5,82.41667v7.16667c0,5.934 -4.816,10.75 -10.75,10.75h-107.5c-5.934,0 -10.75,-4.816 -10.75,-10.75v-7.16667c0,-5.934 4.816,-10.75 10.75,-10.75h107.5c5.934,0 10.75,4.816 10.75,10.75z"
                                /><path
                                    d="M150.5,125.41667v7.16667c0,5.934 -4.816,10.75 -10.75,10.75h-107.5c-5.934,0 -10.75,-4.816 -10.75,-10.75v-7.16667c0,-5.934 4.816,-10.75 10.75,-10.75h107.5c5.934,0 10.75,4.816 10.75,10.75z"
                                /></g
                            ></g
                        ><path
                            d="M0,172v-172h172v172z"
                            fill="none"
                            stroke="none"
                            stroke-width="1"
                            stroke-linejoin="miter"
                        /><g
                            fill="#cccccc"
                            stroke="none"
                            stroke-width="1"
                            stroke-linejoin="miter"
                            ><g
                                ><path
                                    d="M139.75,28.66667h-107.5c-5.934,0 -10.75,4.816 -10.75,10.75v7.16667c0,5.934 4.816,10.75 10.75,10.75h107.5c5.934,0 10.75,-4.816 10.75,-10.75v-7.16667c0,-5.934 -4.816,-10.75 -10.75,-10.75z"
                                /><path
                                    d="M139.75,71.66667h-107.5c-5.934,0 -10.75,4.816 -10.75,10.75v7.16667c0,5.934 4.816,10.75 10.75,10.75h107.5c5.934,0 10.75,-4.816 10.75,-10.75v-7.16667c0,-5.934 -4.816,-10.75 -10.75,-10.75z"
                                /><path
                                    d="M139.75,114.66667h-107.5c-5.934,0 -10.75,4.816 -10.75,10.75v7.16667c0,5.934 4.816,10.75 10.75,10.75h107.5c5.934,0 10.75,-4.816 10.75,-10.75v-7.16667c0,-5.934 -4.816,-10.75 -10.75,-10.75z"
                                /></g
                            ></g
                        ><path
                            d=""
                            fill="none"
                            stroke="none"
                            stroke-width="1"
                            stroke-linejoin="miter"
                        /><path
                            d=""
                            fill="none"
                            stroke="none"
                            stroke-width="1"
                            stroke-linejoin="miter"
                        /></g
                    ></g
                ></svg
            >
            <img
                src="https://img.icons8.com/carbon-copy/100/000000/delete-sign.png"
                alt=""
                class="toggle hidden"
                width="40"
                height="40"
            />
        </button>
    </div>
    <!-- links -->
    <div
        class="toggle hidden md:flex w-full md:w-auto text-right text-bold mt-5 md:mt-0 border-t-2 border-red-900 md:border-none"
    >
        <a
            href="/"
            class="block md:inline-block text-gray-50 hover:text-blue-500 px-3 py-3 border-b-2 border-red-900 md:border-none"
        >
            <span> Home</span></a
        >
        <a
            href="/about"
            class="block md:inline-block text-gray-50 hover:text-blue-500 px-3 py-3 border-b-2 border-red-900 md:border-none"
            ><span>About</span></a
        >
        <a
            href="/events"
            class="block md:inline-block text-gray-50 hover:text-blue-500 px-3 py-3 border-b-2 border-red-900 md:border-none"
        >
            <span>Events</span></a
        >
        <a
            href="/our_boxers"
            class="block md:inline-block text-gray-50 hover:text-blue-500 px-3 py-3 border-b-2 border-red-900 md:border-none"
            ><span>Our Boxers</span></a
        >
    </div>
</nav>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Alfa+Slab+One&display=swap");
    nav {
        border-bottom: gray solid 1px;
        margin-top: -15px;
    }
    a > * {
        font-family: "Alfa Slab One", cursive;
        color: lightgray;
    }
    a > *:hover {
        color: red;
    }
</style>
