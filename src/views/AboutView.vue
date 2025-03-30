<template>
  <div class="about">
    <h1>About Jobs</h1>
    <p>At our company, we offer exciting career opportunities that provide the chance to work on innovative projects, collaborate with talented teams, and grow your skills in the tech industry.</p>
    
    <p>We believe in a culture of learning and development. Whether you're an experienced professional or just starting out, there’s a place for you to thrive.</p>
    
    <p>Here are some of the exciting job roles you can pursue with us:</p>
    <ul>
      <li><strong>UX/UI Designer:</strong> Focus on creating intuitive user interfaces and seamless user experiences.</li>
      <li><strong>Frontend Web Developer:</strong> Build responsive websites with the latest technologies like Vue.js and React.</li>
      <li><strong>Mobile App Developer:</strong> Develop mobile apps for iOS and Android using frameworks like React Native or Flutter.</li>
    </ul>
    
    <p>We’re always looking for passionate individuals to join our team. Apply today!</p>
  </div>
</template>

<script>
export default {
  name: "About",
};
</script>

<style scoped>
.about {
  background-color: #f7f7f7;
  padding: 20px;
  border-radius: 10px;
  margin: 20px auto;
  max-width: 800px;
  font-family: Arial, sans-serif;
}

h1 {
  color: #2c3e50;
  font-size: 2rem;
  margin-bottom: 20px;
}

p {
  font-size: 1rem;
  line-height: 1.6;
  color: #34495e;
  margin-bottom: 10px;
}

ul {
  list-style-type: none;
  padding-left: 0;
}

ul li {
  font-size: 1.1rem;
  margin-bottom: 8px;
  color: #2980b9;
}

ul li strong {
  color: #1abc9c;
}
</style>
