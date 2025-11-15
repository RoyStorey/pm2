<script>
  import '../app.css'
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

