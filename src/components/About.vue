<template>
  <section class="about">
    <h1>About Me</h1>
    <p>
      I am a passionate Data Scientist with a strong background in statistics, machine learning, and data analysis. 
      My journey in data science began with a fascination for uncovering insights from data and transforming them into actionable strategies.
    </p>
    <h2>Skills</h2>
    <ul>
      <li>Python</li>
      <li>R</li>
      <li>Machine Learning</li>
      <li>Data Visualization</li>
      <li>SQL</li>
      <li>Deep Learning</li>
      <li>Big Data Technologies</li>
    </ul>
    <h2>Background</h2>
    <p>
      I hold a degree in Computer Science and have worked on various projects involving predictive modeling, 
      data mining, and statistical analysis. I am always eager to learn new techniques and tools to enhance my skill set.
    </p>
  </section>
</template>

<script>
export default {
  name: 'About'
}
</script>

<style scoped>
.about {
  padding: 20px;
  background: #e0e0e0;
  border-radius: 20px;
  box-shadow: 10px 10px 20px #b0b0b0, -10px -10px 20px #ffffff;
}
h1, h2 {
  color: #333;
}
p, ul {
  color: #555;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  margin: 5px 0;
}
</style>