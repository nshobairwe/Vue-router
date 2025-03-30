<template>
  <div id="nav">
    <router-link to="/">Home</router-link> 
    <router-link to="/about">About</router-link>
    <router-link to="/jobs">Jobs</router-link>
  </div>

  <div class="button-container">
    <button class="redirect-button" @click="redirect">Redirect</button>
    <button class="back-button" @click="back">Go back</button>
  </div>

  <router-view/>
</template>

<script>
export default{
  methods: {
    redirect () {
      this.$router.push({name: 'home'})
    },
    back () {
      this.$router.go(-1)
    },
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
  margin-top: 40px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
  padding: 5px;
  border-radius: 4px;
}

#nav a.router-link-exact-active {
  color: white;
  background: crimson;
}

/* Container for buttons */
.button-container {
  position: fixed;
  top: 10px;
  left: 10px;
  display: flex; /* Align buttons horizontally */
  gap: 10px; /* Space between buttons */
}

button {
  padding: 5px;
  border: none;
  border-radius: 4px;
}

.redirect-button, .back-button {
  background-color: #1abc9c;
  color: white;
}
</style>
