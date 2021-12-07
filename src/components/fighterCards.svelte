<script>
    let amatureFighterArr = [
        {
            id: 1,
            name: "Kevin Soltero",
            dob: "5/27/2005",
            ringName: null,
            weightClass: "107lbs",
            imageUrl: "kevinSoltero.jpeg",
            homeTown: "Kansas City, MO",
            favColor: "Black",
            favSong: "El Karma by Ariel Camacho",
            favMovie: "Ford vs Ferrari",
            threeWords: "Dedicated, Athletic, and Chill",
            favQuote:
                '"I hated every minute of traning, but I said, don\'t quit. Suffer now and live the rest of your life a Champion."',
            boxingGoals: [
                "Get in Shape",
                "Win a couple Tournaments",
                "Become a World Champion",
            ],
        },
        {
            id: 2,
            name: "Lex-Xavier Oliver",
            dob: "02/04/1999",
            ringName: null,
            weightClass: "Heavy Weight",
            imageUrl: "lex-xavierOliver.jpeg",
            homeTown: "Kansas City, MO",
            favColor: "Blue",
            favSong: "Shine by Meek-Mill",
            favMovie: null,
            threeWords: "Dedicated, Hard Worker, and Funny",
            favQuote: '"Shoulders back, chin up."',
            boxingGoals: ["Become a World Champion"],
        },
    ];
    const professionalFighterArr = [
        {
            id: 1,
            name: "Calvin Lynn Metcalf II",
            dob: "12/13/1994",
            ringName: null,
            weightClass: "165lbs",
            imageUrl: "calvinMetcalII.jpeg",
            homeTown: "Kansas City, MO",
            favColor: "Green",
            favSong: null,
            favMovie: "Enter The Dragon",
            threeWords: "Cool, Calm, and Collected",
            favQuote:
                '"There are only two tyepes of people, trained and untrained"',
            boxingGoals: ["To become an undisputed World Champion"],
        },
        {
            id: 2,
            name: 'Edward "Red" Guinn',
            dob: "06/15/1992",
            ringName: null,
            weightClass: "141lbs",
            imageUrl: "edwardGuinn.jpeg",
            homeTown: "Kansas City, MO",
            favColor: null,
            favSong: null,
            favMovie: null,
            threeWords: null,
            favQuote: null,
            boxingGoals: null,
        },
        {
            id: 3,
            name: "Marcus Cole Garza",
            dob: "12/12/1996",
            ringName: "Machismo",
            weightClass: "147-154lbs",
            imageUrl: "marcusGarza.jpeg",
            homeTown: "SAint Joseph, MO",
            favColor: "Lime Green",
            favSong: null,
            favMovie: "End of Watch",
            threeWords: "Loyal, Dedicated and Motivated",
            favQuote: '"Never forget where you came from"',
            boxingGoals: [
                "Be the best I can be pound for pound",
                "Become a World Champion",
            ],
        },
        {
            id: 4,
            name: "Noah Kid",
            dob: "06/28/1998",
            ringName: "Hands",
            imageUrl: "noahKidd.jpeg",
            weightClass: "150lbs",
            homeTown: "Kansas City, MO",
            favColor: "Blue",
            favSong: "First Day Out: Tee Grizzley",
            favMovie: "Friday",
            threeWords: "Lover, Fighter, and Helpful",
            favQuote:
                '"Ain\'t nothing but work out here, you just got to put it in"',
            boxingGoals: ["To become a G.O.A.T."],
        },
        {
            id: 5,
            name: "Ira Sean Johnson",
            dob: "01/01/1991",
            ringName: null,
            weightClass: "148lbs",
            imageUrl: "iraJohnson.jpeg",
            homeTown: "Las Vegas, NV",
            favColor: "Red",
            favSong: null,
            favMovie: null,
            threeWords: "Explosive, Energetic, and Fearless",
            favQuote: '"Sky\'s the limit, push hard, play hard, and go far"',
            boxingGoals: ["To be the best fighter I can be"],
        },
    ];
</script>

<h2>Amateure</h2>
<hr />
<section>
    {#each amatureFighterArr.filter((u) => u !== null) as amature}
        <div class="fighter-card">
            <ul>
                {#if amature.imageUrl}
                    <div class="center">
                        <li>
                            <img src={amature.imageUrl} alt={amature.name} />
                        </li>
                    </div>
                {/if}
                {#if amature.name}
                    <li>
                        <b><u>Name</u>:</b>
                        {amature.name}
                    </li>
                {/if}
                {#if amature.ringName}
                    <li>
                        <b><u>Ring Name</u>:</b>
                        {amature.ringName}
                    </li>
                {/if}
                {#if amature.dob}
                    <li>
                        <b><u>Date of Birth</u>:</b>
                        {amature.dob}
                    </li>
                {/if}
                {#if amature.weightClass}
                    <li>
                        <b><u>Weight Class</u>:</b>
                        {amature.weightClass}
                    </li>
                {/if}
                {#if amature.homeTown}
                    <li>
                        <b><u>Hometown</u>:</b>
                        {amature.homeTown}
                    </li>
                {/if}
                {#if amature.favColor}
                    <li>
                        <b><u>Favorite Color</u>:</b>
                        {amature.favColor}
                    </li>
                {/if}
                {#if amature.favSong}
                    <li>
                        <b><u>Favorite Song</u>:</b>
                        {amature.favSong}
                    </li>
                {/if}
                {#if amature.favMovie}
                    <li>
                        <b><u>Favorite Movie</u>:</b>
                        {amature.favMovie}
                    </li>
                {/if}
                {#if amature.threeWords}
                    <li>
                        <b><u>Three Descriptive Words</u>:</b>
                        {amature.threeWords}
                    </li>
                {/if}
                {#if amature.favQuote}
                    <li>
                        <b><u>Favorite Quote</u>:</b>
                        {amature.favQuote}
                    </li>
                {/if}
                {#if amature.boxingGoals}
                    <li>
                        <ul>
                            <b><u>Goals</u>:</b>
                            {#each amature.boxingGoals as goals}
                                <li>
                                    {goals}
                                </li>
                            {/each}
                        </ul>
                    </li>
                {/if}
            </ul>
        </div>
    {/each}
</section>
<br />
<br />
<h2>Professional</h2>
<hr />
<section>
    {#each professionalFighterArr as pro (pro.id)}
        <div class="fighter-card">
            <ul>
                {#if pro.imageUrl}
                    <div class="center">
                        <li>
                            <img src={pro.imageUrl} alt={pro.name} />
                        </li>
                    </div>
                {/if}
                {#if pro.name}
                    <li>
                        <b><u>Name</u>:</b>
                        {pro.name}
                    </li>
                {/if}
                {#if pro.ringName}
                    <li>
                        <b><u>Ring Name</u>:</b>
                        {pro.ringName}
                    </li>
                {/if}
                {#if pro.dob}
                    <li>
                        <b><u>Date of Birth</u>:</b>
                        {pro.dob}
                    </li>
                {/if}
                {#if pro.weightClass}
                    <li>
                        <b><u>Weight Class</u>:</b>
                        {pro.weightClass}
                    </li>
                {/if}
                {#if pro.homeTown}
                    <li>
                        <b><u>Hometown</u>:</b>
                        {pro.homeTown}
                    </li>
                {/if}
                {#if pro.favColor}
                    <li>
                        <b><u>Favorite Color</u>:</b>
                        {pro.favColor}
                    </li>
                {/if}
                {#if pro.favSong}
                    <li>
                        <b><u>Favorite Song</u>:</b>
                        {pro.favSong}
                    </li>
                {/if}
                {#if pro.favMovie}
                    <li>
                        <b><u>Favorite Movie</u>:</b>
                        {pro.favMovie}
                    </li>
                {/if}
                {#if pro.threeWords}
                    <li>
                        <b><u>Three Descriptive Words</u>:</b>
                        {pro.threeWords}
                    </li>
                {/if}
                {#if pro.favQuote}
                    <li>
                        <b><u>Favorite Quote</u>:</b>
                        {pro.favQuote}
                    </li>
                {/if}
                {#if pro.boxingGoals}
                    <li>
                        <ul>
                            <b><u>Goals</u>:</b>
                            {#each pro.boxingGoals as goals}
                                <li>
                                    {goals}
                                </li>
                            {/each}
                        </ul>
                    </li>
                {/if}
            </ul>
        </div>
    {/each}
</section>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Azeret+Mono:wght@100&display=swap");

    :global(body) {
        background-color: black;
        color: grey;
    }

    section {
        font-family: "Azeret Mono", monospace;

        max-width: 700px;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }
    h2 {
        font-size: xx-large;
        text-align: left;
        font-family: "Alfa Slab One", cursive;
        margin-bottom: 20px;
        margin-top: 20px;
    }
    img {
        border-radius: 4px;
        margin-bottom: 10px;
        width: 275px;
        height: 325px;
        border: solid 2px slategrey;
    }
    .fighter-card {
        margin: 10px;
        width: 325px;
        height: 735px;
        color: white;
        background: rgb(128, 128, 128);
        background: linear-gradient(
            225deg,
            rgba(128, 128, 128, 1) 0%,
            rgba(9, 9, 121, 0) 70%,
            rgba(128, 128, 128, 1) 100%
        );
        border-radius: 4px;
        display: flex;
        justify-content: center;
        font-size: small;
        border: slategrey 2px solid;
    }
    .fighter-card > * {
        margin: 10px;
    }
    .center {
        display: flex;
        justify-content: center;
        margin: 1em;
    }
    hr {
        margin-top: -20px;
        margin-bottom: 20px;
        width: 250px;
        color: gray;
        background-color: gray;
        border-color: gray;
    }
</style>
