<script>
  import "../app.css";
  const loggedInUser = {
    name: "Vladimir Romanov",
    team: "Manager",
    profileImageUrl: "/image.png",
  };
  const bonkoUrl = "/bonkotm2.png";
</script>

<div class="header">
  <div class="logo">
    <img class="bonkoLogo" src={bonkoUrl} alt="Bonko TM2" />
  </div>
  <div class="profile-holder">
    <div class="side">
      <h4>{loggedInUser.name}</h4>
      <h5>{loggedInUser.team}</h5>
    </div>
    <div class="side circle">
      <img
        class="usericon"
        src={loggedInUser.profileImageUrl}
        alt={loggedInUser.name}
      />
    </div>
  </div>
</div>
