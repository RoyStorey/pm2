<div class="header">
  <div class="logo">
    <h2>Bonko TM^2</h2>
  </div>
  <div class="profile-holder">
    <div class="side">
      <h4>Vladimir Romanov</h4>
      <h5>Manager</h5>
    </div>
    <div class="side">
      <img src="img" />
    </div>
  </div>
</div>

<style>

.header {
	padding: 1rem 2rem;
  height:min-content;
	/* background-color: red; */
  display:flex;
  flex-direction: row;
  justify-content: space-between;
  outline:1px solid black;
}
.profile-holder{
  display:flex;
  flex-direction: row;
}
.side{
  display:flex;
  flex-direction: column;
  text-align: right;
}
.side h4,h5{
  margin:0px;
}
</style>