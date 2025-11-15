<script>
  import './app.css';
  import Header from './components/header.svelte';
  import OnlineCircles from './components/onlineCircles.svelte';
  import NavBar from './components/navBar.svelte';
  import NumberOfProjects from './components/numberOfProjects.svelte';
  import NextDeadline from './components/nextDeadline.svelte';
  import ProjectsList from './components/projectsList.svelte';
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
  </div>
</div>

<style>
.content{
  width:100%;
  height:min-content;
  outline:1px solid black;
  display:flex;
  flex-direction: row;

}
.side{
  display:flex;
  flex-direction: column;
  outline:1px solid black;
}
.left{
  display:flex;
  flex-grow: 1;
}
.right{
  display:flex;
  flex-grow:1;
}

</style>
