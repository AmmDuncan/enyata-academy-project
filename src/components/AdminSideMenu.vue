<template>
  <div class="side-menu">
    <div class="user-details">
      <div>
        <img
          src="../assets/svgs/admin-profile.svg"
          alt="admin profile picture"
        />
      </div>
      <p class="user-name">Jane Doe</p>
      <p class="user-email">doe@enyata.com</p>
    </div>
    <div class="nav-buttons">
      <router-link to="/admin-dashboard">
        <img
          src="../assets/svgs/dashboard-logo.svg"
          alt="dashboard icon"
          class="nav-button-img"
        />Dashboard
      </router-link>
      <router-link to="/create-application">
        <img
          src="../assets/svgs/upload.svg"
          alt="create application icon"
          class="nav-button-img"
        />Create Application
      </router-link>
      <router-link to="/application-entries">
        <img
          src="../assets/svgs/application-entries.svg"
          alt="application entries(download) icon"
          class="nav-button-img"
        />Application Entries
      </router-link>
      <router-link to="/compose-assessment">
        <img
          src="../assets/svgs/note.svg"
          alt="compose assessment icon"
          class="nav-button-img"
        />Compose Assessment
      </router-link>
      <router-link to="/assessment-history">
        <img
          src="../assets/svgs/history.svg"
          alt="clock winding back(history) icon"
          class="nav-button-img"
        />Assessment History
      </router-link>
      <router-link to="/results">
        <img
          src="../assets/svgs/results.svg"
          alt="results icon"
          class="nav-button-img"
        />Results
      </router-link>
      <router-link to="/settings">
        <img
          src="../assets/svgs/settings.svg"
          alt="seetings icon"
          class="nav-button-img"
        />Settings
      </router-link>
      <router-link to="/logout" class="logout-button">
        <img
          src="../assets/svgs/logout-logo.svg"
          alt="logout icon"
          class="nav-button-img"
        />Log Out
      </router-link>
    </div>
  </div>
  <router-view />
</template>

<script>
export default {
  name: "AdminSideMenu",
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,100;0,300;0,400;0,700;0,900;1,100;1,300;1,400;1,700;1,900&display=swap");
* {
  font-family: "Lato", sans-serif;
  font-size: 16px;
}
.side-menu {
  max-width: 292px;
  box-shadow: 0px 5px 15px rgba(33, 31, 38, 0.05);
  height: auto;
  height: 100vh;
  position: fixed;
}
.user-details {
  background-color: #7557d3;
  padding: 57px 91px;
  text-align: center;
  color: #ffffff;
  letter-spacing: -0.02em;
  margin-bottom: 28px;
}
.user-name {
  margin: 13px 0 5px;
  font-weight: 700;
  font-size: 20px;
}
.user-email {
  font-style: italic;
  font-weight: 400;
}
.logout-button {
  margin-top: 50px;
}
.nav-button-img {
  margin-right: 16.56px;
}
.nav-buttons a {
  height: 49px;
  display: block;
  background-color: #ffffff;
  color: #2b3c4e;
  outline: none;
  border: none;
  border-left: 4px solid #ffffff;
  padding-left: 30px;
  cursor: pointer;
  line-height: 19.2px;
  text-align: left;
  width: 100%;
  display: flex;
  align-items: center;
}
a.router-link-exact-active {
  border-left: 4px solid #7557d3;
  font-weight: 700;
}
a {
  text-decoration: none;
}
.assessment-button {
  margin: 28px 0 57px;
}
</style>