<template>
    <div v-if="job" class="job-container">
      <h1 class="job-title">{{ job.title }}</h1>
      <p class="job-id">Job ID: {{ id }}</p>
      <p class="job-details">{{ job.details }}</p>
    </div>
    <div v-else class="loading-container">
      <p>Loading job details...</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        id: this.$route.params.id,
        job: null
      };
    },
    mounted() {
      fetch('http://localhost:3000/jobs/' + this.id)
        .then((res) => res.json())
        .then(data => this.job = data)
        .catch(err => console.log(err.message));
    }
  }
  </script>
  
  <style scoped>
  .job-container {
    max-width: 800px;
    margin: 20px auto;
    padding: 20px;
    background-color: #f9f9f9;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }
  
  .job-title {
    font-size: 2em;
    color: #333;
    font-weight: bold;
    margin-bottom: 15px;
  }
  
  .job-id {
    font-size: 1.1em;
    color: #666;
    margin-bottom: 20px;
  }
  
  .job-details {
    font-size: 1.2em;
    line-height: 1.6;
    color: #444;
    font-family: 'Arial', sans-serif;
  }
  
  .loading-container {
    text-align: center;
    font-size: 1.5em;
    color: #888;
  }
  </style>
  