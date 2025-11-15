<script>
  const Users = [
    { name: "Vladimir Romanov", status: "online" },
    { name: "Elena Markova", status: "away" },
    { name: "Damian Turell", status: "offline" },
    { name: "Sabrina Holt", status: "online" },
    { name: "Marcus Levingston", status: "away" },
    { name: "Aria Bennett", status: "online" },
    { name: "Jasper Caldwell", status: "offline" },
    { name: "Lydia Serrano", status: "away" },
    { name: "Theodore Graves", status: "online" },
    { name: "Nina Falk", status: "offline" },
  ];
</script>

<div class="online-container">
  {#each Users as user}
    <div class="circle {user.status}">
      <h1>{user.name[0]}</h1>
    </div>
  {/each}
</div>

<style>
  .online-container {
    display: flex;
    flex-direction: row;
    gap: 1rem;
    padding: 1rem;
    justify-content: space-evenly;
  }
  .circle {
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 100%;
    outline: 1px solid black;
    aspect-ratio: 1 / 1;
    height: 4rem;
    color: black;
    user-select: none;
  }

  .online {
    background-color: #00e700;
  }
  .offline {
    background-color: #848484;
  }
  .away {
    background-color: #ffe100;
  }
</style>
