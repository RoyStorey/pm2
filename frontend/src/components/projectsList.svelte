<script>
  const projects = [
    { name: "Project Atlas", status: "active" },
    { name: "Project Nebula", status: "queue" },
    { name: "Project Horizon", status: "missed" },
    { name: "Project Echo", status: "active" },
    { name: "Project Ironclad", status: "queue" },
    { name: "Project Solstice", status: "active" },
    { name: "Project Catalyst", status: "missed" },
    { name: "Project Vanguard", status: "queue" },
    { name: "Project Phoenix", status: "active" },
    { name: "Project Polaris", status: "missed" },
  ];
</script>

<div class="projects-list">
  {#each projects as project}
    <div class="project {project.status}">
      <h2>+</h2>
      <h2 class="project-title">{project.name}</h2>
    </div>
  {/each}
</div>

<style>
  .projects-list {
    height: 100%;
    max-height: 100%;
    overflow-y: scroll;
    /* background-color:rgb(184, 255, 184); */
    outline: 1px solid black;
    padding: 1rem;
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }
  .project {
    display: flex;
    flex-direction: row;
    gap: 2rem;
    padding: 1rem;
  }
  .active {
    background-color: #81ee56b6;
  }
  .missed {
    background-color: #d53f3f77;
  }
  .queue {
    background-color: #00b0eabd;
  }
  h2 {
    margin: 0px;
    color: White;
  }
  .project-title {
    color: black;
    font-weight: 400;
  }
</style>
