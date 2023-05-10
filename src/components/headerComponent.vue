<script>
export default {
  name: 'headerComponent'
}

</script>

<template>
  <header>
    <nav>
      <div>
        <img src="../assets/Logo.png" alt="logo">
      </div>
      <RouterLink to="/overview">Overview</RouterLink>
      <RouterLink to="/movies">Movies</RouterLink>
      <RouterLink to="/upload">Upload</RouterLink>
      <RouterLink to="/Reporting">Reporting</RouterLink>
      <RouterLink to="/users">Users</RouterLink>
    </nav>
    <div class="icons">
      <div>
        <img class="icon" src="../assets/icons/iconSetting.png" alt="">
      </div>
      <div>
        <img class="icon" src="../assets/icons/iconNotification.png" alt="">
      </div>
      <div>
        <img src="../assets/images/Avatar.jpg" alt="" class="profilepic">
      </div>
    </div>
  </header>
</template>

<style scoped>

header {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  background: #000000;
  width: 85.4rem;
  height: 4.5em;
}
nav {
  padding-left: 5em;
  display: grid;
  grid-template-columns: repeat(6,1fr);
  display: flex;
  justify-content: space-between;
  gap: 1em;
}
nav a {
  font-family: 'Helvetica Neue';
  font-style: normal;
  font-weight: 500;
  font-size: 1rem;
  color: #6A6A6A;
  line-height: 2.3em;
}
nav a:hover, nav a:focus {
  color: #FFFFFF;
}
.icons {
  display: flex;
  gap: 1em;
  padding-right: 5em;
}
.profilepic {
  width: 2em;
  height: 2em;
  border-radius: 100%;
}
.icon {
  margin-top: 0.4em;
}
@media (min-width: 1024px) {
  
}
</style>
