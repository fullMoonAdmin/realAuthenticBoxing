<script>
    import Button from "../components/button.svelte";
</script>

<section
    class="relative h-screen flex flex-col items-center justify-center text-center text-white py-0 px-3"
>
    <div
        class="video-docker absolute top-0 left-0 w-full h-full overflow-hidden "
        id="docker"
    >
        <!--<video
            poster=""
            class="min-w-full min-h-full absolute object-cover"
            src="shortBoxingCinematic.mp4"
            type="video/mp4"
            autoplay
            muted
            loop
        />-->
        <img src="banner.jpg" alt="boxing" class="min-w-full min-h-full " />
    </div>

    <div class="video-content">
        <!-- 
            <Button />
        --> 
        <h1>Authentic Boxing</h1>
    </div>
</section>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Alfa+Slab+One&display=swap");

    .video-docker video {
        top: 45%;
        left: 50%;
        transform: translate(-50%, -50%);
        margin-bottom: -20px;
    }

    .video-content {
        z-index: 2;
    }
    h1 {
        position: absolute;
        top: 70px;
        left: 20px;
        color: rgba(192, 192, 192, 0.616);
        z-index: 0;
        font-size: 3.5em;
        font-family: "Alfa Slab One", cursive;
        -webkit-text-stroke: 1px black;
    }

    #docker {
        background-color: black;
        margin-bottom: -20px;
        height: 100%;
    }
</style>
