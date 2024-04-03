<template>
  <div id="app">
    <!-- Navigation Links -->
    <div class="navbar">
      <router-link to="/" class="nav-item">Home</router-link>
      <router-link to="/about" class="nav-item">About</router-link>
      <router-link to="/gallery" class="nav-item">Gallery</router-link>
      <router-link to="/events" class="nav-item">Events</router-link>
      <router-link to="/hobbies" class="nav-item">Hobbies</router-link>
    </div>

    <!-- Route Content -->
    <router-view />
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
body, #app {
  margin: 0;
  padding: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  background-image: url('@/assets/tyBG.jpg');
  background-size: cover; /* Cover the entire screen */
}

.navbar {
  background-image: url('@/assets/tyBG.jpg');
  /* Ensure the background image exactly fits the header size */
  background-repeat: no-repeat; /* Prevent repeating the background image */
  display: flex;
  justify-content: space-around;
  align-items: center;
  padding: 10px 0;
}

.nav-item {
  text-decoration: none;
  color: #ffffff;
  padding: 10px 20px;
  border-radius: 5px;
  transition: transform 0.3s ease; /* Add transition for smooth hover effect */
  font-weight: bold; /* Make the font bold */
  font-size: 1.1rem; /* Adjust the font size as needed */
}

.nav-item:hover {
  background-color: #00d9fff1;
  transform: scale(1.1); /* Enlarge the nav-item when hovered over */
}
</style>
