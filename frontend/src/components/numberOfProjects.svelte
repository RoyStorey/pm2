<script>
  const projects = { total: 12, queue: 4, active: 6, inactive: 2 };
</script>

<div class="projects">
  <p>
    <b class="total">{projects.total}</b> Total Projects
  </p>
  <p>
    <b class="queue">{projects.queue}</b> In Queue
  </p>
  <p>
    <b class="active">{projects.active}</b> Active Projects
  </p>
  <p>
    <b class="inactive">{projects.inactive}</b> Inactive Projects
  </p>
</div>

<style>
  .projects {
    outline: 1px solid black;
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
  }
  .total {
    color: black;
  }
  .queue {
    color: blue;
  }
  .active {
    color: green;
  }
  .inactive {
    color: red;
  }
</style>
