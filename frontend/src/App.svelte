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

<style>
  .content {
    width: 100%;
    height: 85vh;
    outline: 1px solid black;
    display: flex;
    flex-direction: row;
  }
  .side {
    display: flex;
    flex-direction: column;
    outline: 1px solid black;
  }
  .left {
    width: 50%;
  }
  .right {
    width: 50%;
  }
  .calendar {
    background-color: #212121;
    display: flex;
    justify-content: center;
    padding: 0.5rem;
    height: 100%;
  }
  .ec {
    min-height: 100%;
    width: 90%;
    /* https://github.com/vkurko/calendar/blob/master/packages/core/src/styles/theme.scss */
    --ec-bg-color: #212121;
    --ec-text-color: #ffffff;
    --ec-border-color: #212121;
  }
</style>
