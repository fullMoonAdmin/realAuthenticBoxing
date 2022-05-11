<script>
  import Map from "../components/map.svelte";

  import Contact from "../components/contact.svelte";
</script>

<main>
  <h1>Authentic Boxing</h1>
  <div class="flex-container">
    <h2>The Venue</h2>
    <img src="gymFront.JPG" id="gym" alt="gym building" />
    <Map />
    <h2 id="seat">Seat Map</h2>
    <img
      src="seatingChartPlain.svg"
      id="seatingPlan"
      alt="seat map for venue"
    />
    <h2>Concessions Menu</h2>

    <Contact />
  </div>
</main>

<style>
  main {
    margin-top: 50px;
    margin-bottom: 70px;
    color: gray;
    font-family: "Alfa Slab One", cursive;
  }
  h1 {
    font-size: 50px;
    margin-left: 0.5em;
  }
  h2 {
    font-size: 40px;
  }
  #seat {
    margin-top: 75px;
  }
  #gym {
    margin: 1rem;
    width: 40rem;
    border-radius: 4px;
    border: solid 2px gray;
  }
  #seatingPlan {
    width: 60rem;
    border-radius: 4px;
    border: solid 2px gray;
    background-color: antiquewhite;
    margin: 1rem;
  }
  .flex-container {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
  }
</style>
