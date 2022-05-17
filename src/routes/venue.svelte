<script>
  import Map from "../components/map.svelte";

  import Contact from "../components/contact.svelte";
</script>

<main>
  <h1>Authentic Boxing</h1>
  <div class="flex-container">
    <h2>The Venue</h2>
    <img src="seatingChart.svg" id="seatingPlan" alt="seat map for venue" />
    <Map />
    <!--
    <h2>Concessions Menu</h2>
-->
    <Contact />
  </div>
</main>

<style>
  main {
    margin-top: 50px;
    margin-bottom: 70px;
    color: gray;
    font-family: "Alfa Slab One", cursive;
    background-color: black;
  }
  h1 {
    font-size: 50px;
    margin-left: 0.5em;
  }
  h2 {
    margin-top: 80px;
    font-size: 40px;
  }
  
  #seatingPlan {
    width: 75rem;
    border-radius: 4px;
    border: solid 2px gray;
    background-color: hsla(100, 100%, 100%, 50%);
    margin: 1rem;
  }
  .flex-container {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
  }
</style>
