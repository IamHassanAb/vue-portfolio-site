<template>
  <div class="home">
    <h1>Welcome to My Portfolio</h1>
    <p>
      I am a person
    </p>
    <p>
      Explore my <a href="#projects"><span>projects</span></a> and learn more about my skills and experience.
    </p>
  </div>
</template>

<script>
export default {
  name: 'Home',
}
</script>

<style scoped>
.home {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  text-align: center;
  color: #333;
  background: #e0e0e0; /* Light background for neumorphism */
  border-radius: 20px;
  box-shadow: 8px 8px 20px #b8b8b8, 
              -8px -8px 20px #ffffff; /* Neumorphism effect */
  padding: 20px;
}
</style>