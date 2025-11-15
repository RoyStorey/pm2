<script>
  import '../app.css'
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