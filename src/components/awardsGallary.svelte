<script>
  const awardArr = [
    "/awards/metcalf1.jpeg",
    "/awards/metcalf2.jpeg",
    "/awards/metcalf3.jpeg",
    "/awards/metcalf4.jpeg",
    "/awards/metcalf5.jpeg",
    "/awards/metcalf6.jpeg",
    "/awards/burnett1.jpeg",
    "/awards/kidd1.jpeg",
    "/awards/gonzales1.jpeg",
    "/awards/henley1.jpeg",
    "/awards/perez1.jpeg",
    "/awards/walker1.jpeg",
    "/awards/jimenez1.jpeg",
    "/awards/soltero1.jpeg",
  ];
</script>

<div id="awardGallary">
  {#each awardArr as award}
    <img src={award} alt="award" />
  {/each}
</div>

<style>
  img {
    border: 1px solid white;
    width: 25rem;
    margin: 0.5rem;
    border-radius: 4px;
  }

  #awardGallary {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    flex-direction: row;
  }
</style>
