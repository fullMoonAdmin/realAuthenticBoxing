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
                "Becone a World Champion",
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
            boxingGoals: ["Becone a World Champion"],
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
            favQuote: "Ksy's the limit, push hard, play hard, and go far",
            boxingGoals: ["To be the best fighter I can be"],
        },
    ];
</script>

<section>
    <h2>Amature</h2>
    {#each amatureFighterArr as amature (amature.id)}
        <div class="fighter-card">
            <ul>
                <li>
                    <img src={amature.imageUrl} alt={amature.name} />
                </li>
                <li>
                    Name: {amature.name}
                </li>

                <li>
                    Ring Name: {amature.ringName}
                </li>

                <li>
                    Date of Birth: {amature.dob}
                </li>
                <li>
                    Weight Class: {amature.weightClass}
                </li>
                <li>
                    Hometown: {amature.homeTown}
                </li>
                <li>
                    Favorite Color: {amature.favColor}
                </li>
                <li>
                    Favorite Song: {amature.favSong}
                </li>
                <li>
                    Three Descriptive Words: {amature.threeWords}
                </li>
                <li>
                    Favorite Quote: {amature.favQuote}
                </li>
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
            </ul>
        </div>
    {/each}
</section>
<section>
    <h2>Professional</h2>
    {#each professionalFighterArr as pro (pro.id)}
        <div class="fighter-card">
            <ul>
                <li>
                    <img src={pro.imageUrl} alt={pro.name} />
                </li>
                <li>
                    Name: {pro.name}
                </li>

                <li>
                    Ring Name: {pro.ringName}
                </li>

                <li>
                    Date of Birth: {pro.dob}
                </li>
                <li>
                    Weight Class: {pro.weightClass}
                </li>
                <li>
                    Hometown: {pro.homeTown}
                </li>
                <li>
                    Favorite Color: {pro.favColor}
                </li>
                <li>
                    Favorite Song: {pro.favSong}
                </li>
                <li>
                    Three Descriptive Words: {pro.threeWords}
                </li>
                <li>
                    Favorite Quote: {pro.favQuote}
                </li>
                <li />
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
    }
    h2 {
        font-size: x-large;
    }
    h1 {
        font-size: 45px;
    }
    .fighter-card {
        margin: 10px;
        width: 325px;
        height: 800px;
        color: white;
        background-color: rgba(128, 128, 128, 0.425);
        border-radius: 4px;
        display: flex;
        justify-content: center;
    }
    .fighter-card > * {
        margin: 10px;
    }
</style>
