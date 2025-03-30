<template>
  <div class="home">
    <h1>Welcome to Our Careers Page</h1>
    <p>Are you looking to join a dynamic and innovative team? We offer exciting job opportunities where you can grow your career and contribute to impactful projects.</p>
    
    <p>Whether you are a UX/UI Designer, Frontend Web Developer, or a Mobile App Developer, we have a variety of roles available. We believe in fostering a collaborative work environment and supporting professional development.</p>
    
    <p>Explore our job listings today and apply to be part of our team!</p>
    
    <button class="cta-button" @click="redirectToJobs">View Job Listings</button>
  </div>
</template>

<script>
export default {
  name: 'HomeView',
  methods: {
    redirectToJobs() {
      this.$router.push({ name: 'Jobs' }); // Adjust the route name as per your router setup
    }
  }
}
</script>

<style scoped>
.home {
  background-color: #f5f5f5;
  padding: 30px;
  border-radius: 10px;
  margin: 20px auto;
  max-width: 900px;
  font-family: Arial, sans-serif;
  text-align: center;
}

h1 {
  color: #2c3e50;
  font-size: 2.5rem;
  margin-bottom: 20px;
}

p {
  color: #34495e;
  font-size: 1.2rem;
  line-height: 1.6;
  margin-bottom: 20px;
}

.cta-button {
  background-color: #1abc9c;
  color: white;
  padding: 10px 20px;
  font-size: 1.2rem;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.cta-button:hover {
  background-color: #16a085;
}
</style>
