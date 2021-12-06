<script>
    const users = [
        { name: "Benny", favColor: "green" },
        { name: "Orange", favColor: null },
    ];
</script>

{#each users.filter((u) => u !== null) as user}
    <li>{user.name}</li>
    <li>{user.favColor}</li>
{/each}
