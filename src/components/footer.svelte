<script>
    import SocialIcons from "@rodneylab/svelte-social-icons";
</script>

<footer>
    <div
        class="flex flex-row gap-4 justify-end bg-gradient-to-r from-black to-gray-600  "
    >
        <div class="flex flex-row justify-center gap-4 m-1">
            <div id="container">
                <a
                    href="https://www.facebook.com/profile.php?id=100063753182571&ref=page_internal"
                >
                    <SocialIcons
                        alt="Facebook link"
                        network="facebook"
                        width="24"
                        height="24"
                        fgColor="#FFFFFF"
                        bgColor="#0778E8"
                    />
                </a>
            </div>
            <div>
                <span class="text-gray-50"> &copy Authentic Boxing </span>
            </div>
            <div />
        </div>
    </div>
</footer>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Alfa+Slab+One&display=swap");
    footer {
        border-top: gray 1px solid;
        position: fixed;
        width: 100vw;
        max-width: 100%;
        bottom: 0;
        font-family: "Alfa Slab One", cursive;
    }
    span {
        color: lightgray;
    }
    #container:hover {
        animation: createBox 0.5s;
    }
    @keyframes createBox {
        from {
            transform: scale(1);
        }
        to {
            transform: scale(1.25);
        }
    }
</style>
