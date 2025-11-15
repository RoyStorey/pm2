<script>
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

<style>
  .header {
    padding: 1rem 2rem;
    height: 9vh;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    outline: 1px solid black;
  }
  .logo {
    display: flex;
    align-items: center;
  }
  .bonkoLogo {
    max-height: 50%;
  }
  .profile-holder {
    display: flex;
    flex-direction: row;
    gap: 2rem;
    align-items: center;
  }
  .side {
    display: flex;
    flex-direction: column;
    text-align: right;
  }
  .side h4,
  h5 {
    margin: 0px;
  }

  .circle {
    height: 50px;
    width: 50px;
    outline: 1px solid black;
    background-color: rgba(204, 197, 197, 0.377);
    border-radius: 50px;
  }
  .circle .usericon {
    height: 100%;
  }
</style>
