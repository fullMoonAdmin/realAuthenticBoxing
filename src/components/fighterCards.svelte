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
                "I hated every minute of traning, but I said, don't quit. Suffer now and live the rest of your life a Champion.",
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
            favQuote: "Shoulders back, chin up.",
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
                "There are only two tyepes of people, trained and untrained",
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
            favQuote: "Never forget where you came from",
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
                "Ain't nothing but work out here, you just got to put it in",
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
            favQuote: "Sky's the limit, push hard, play hard, and go far",
            boxingGoals: ["To be the best fighter I can be"],
        },
    ];
</script>

<h2>Amature</h2>
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
                        Name: {amature.name}
                    </li>
                {/if}
                {#if amature.ringName}
                    <li>
                        Ring Name: {amature.ringName}
                    </li>
                {/if}
                {#if amature.dob}
                    <li>
                        Date of Birth: {amature.dob}
                    </li>
                {/if}
                {#if amature.weightClass}
                    <li>
                        Weight Class: {amature.weightClass}
                    </li>
                {/if}
                {#if amature.homeTown}
                    <li>
                        Hometown: {amature.homeTown}
                    </li>
                {/if}
                {#if amature.favColor}
                    <li>
                        Favorite Color: {amature.favColor}
                    </li>
                {/if}
                {#if amature.favSong}
                    <li>
                        Favorite Song: {amature.favSong}
                    </li>
                {/if}
                {#if amature.favMovie}
                    <li>
                        Favorite Movie: {amature.favMovie}
                    </li>
                {/if}
                {#if amature.threeWords}
                    <li>
                        Three Descriptive Words: {amature.threeWords}
                    </li>
                {/if}
                {#if amature.favQuote}
                    <li>
                        Favorite Quote: {amature.favQuote}
                    </li>
                {/if}
                {#if amature.boxingGoals}
                    <li>
                        <ul>
                            Goals:
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
                        Name: {pro.name}
                    </li>
                {/if}
                {#if pro.ringName}
                    <li>
                        Ring Name: {pro.ringName}
                    </li>
                {/if}
                {#if pro.dob}
                    <li>
                        Date of Birth: {pro.dob}
                    </li>
                {/if}
                {#if pro.weightClass}
                    <li>
                        Weight Class: {pro.weightClass}
                    </li>
                {/if}
                {#if pro.homeTown}
                    <li>
                        Hometown: {pro.homeTown}
                    </li>
                {/if}
                {#if pro.favColor}
                    <li>
                        Favorite Color: {pro.favColor}
                    </li>
                {/if}
                {#if pro.favSong}
                    <li>
                        Favorite Song: {pro.favSong}
                    </li>
                {/if}
                {#if pro.favMovie}
                    <li>
                        Favorite Movie: {pro.favMovie}
                    </li>
                {/if}
                {#if pro.threeWords}
                    <li>
                        Three Descriptive Words: {pro.threeWords}
                    </li>
                {/if}
                {#if pro.favQuote}
                    <li>
                        Favorite Quote: {pro.favQuote}
                    </li>
                {/if}
                {#if pro.boxingGoals}
                    <li>
                        <ul>
                            Goals:
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
    @import url("https://fonts.googleapis.com/css2?family=Alfa+Slab+One&display=swap");
    :global(body) {
        background-color: black;
        color: grey;
    }

    section {
        font-family: "Alfa Slab One", cursive;

        max-width: 700px;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }
    h2 {
        font-size: xx-large;
        position: inherit;
        text-align: left;
        font-family: "Alfa Slab One", cursive;
    }
    img {
        border-radius: 4px;
        margin-bottom: 10px;
        width: 275px;
        height: 325px;
    }
    .fighter-card {
        margin: 10px;
        width: 325px;
        height: 700px;
        color: white;
        background-color: rgba(128, 128, 128, 0.425);
        border-radius: 4px;
        display: flex;
        justify-content: center;
        font-size: small;
    }
    .fighter-card > * {
        margin: 10px;
    }
    .center {
        display: flex;
        justify-content: center;
        margin: 1em;
    }
</style>
