<script>
  import "./app.css";
  import Header from "./components/header.svelte";
  import OnlineCircles from "./components/onlineCircles.svelte";
  import NavBar from "./components/navBar.svelte";
  import NumberOfProjects from "./components/numberOfProjects.svelte";
  import NextDeadline from "./components/nextDeadline.svelte";
  import ProjectsList from "./components/projectsList.svelte";
  import { Calendar, DayGrid } from "@event-calendar/core";

  let options = $state({
    view: "dayGridMonth",
    events: [],
  });
</script>

<Header />
<div class="content">
  <div class="side left">
    <OnlineCircles />
    <NumberOfProjects />
    <ProjectsList />
  </div>
  <div class="side right">
    <NavBar />
    <NextDeadline />
    <div class="calendar">
      <div class="ec">
        <Calendar plugins={[DayGrid]} {options} />
      </div>
    </div>
  </div>
</div>