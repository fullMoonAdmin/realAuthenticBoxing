<section
    class="relative h-screen flex flex-col items-center justify-center text-center text-white py-0 px-3"
>
    <div
        class="video-docker absolute top-0 left-0 w-full h-full overflow-hidden"
    >
        <video
            poster=""
            class="min-w-full min-h-full absolute object-cover"
            src="shortBoxingCinematic.mp4"
            type="video/mp4"
            autoplay
            muted
            loop
        />
    </div>
    <div class="video-content space-y-2">
        <h1 class="font-light text-6xl">Authentic Boxing</h1>
    </div>
</section>

<style>
    .video-docker video {
        top: 45%;
        left: 50%;
        transform: translate(-50%, -50%);
    }
    .video-docker::after {
        content: "";
        position: absolute;
        width: 100%;
        height: 100%;
        top: 0;
        left: 0;
        background: rgba(0, 0, 0, 0.342);
        z-index: 1;
    }

    .video-content {
        z-index: 2;
    }
</style>
