<template>
  <div class="projects-container">
    <h2>My Projects</h2>
    <div class="project" v-for="project in projects" :key="project.id">
      <h3>{{ project.title }}</h3>
      <p>{{ project.description }}</p>
      <a :href="project.link" target="_blank">View Project</a>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          id: 1,
          title: 'Project One',
          description: 'A brief description of Project One.',
          link: 'https://github.com/user/project-one'
        },
        {
          id: 2,
          title: 'Project Two',
          description: 'A brief description of Project Two.',
          link: 'https://github.com/user/project-two'
        },
        {
          id: 3,
          title: 'Project Three',
          description: 'A brief description of Project Three.',
          link: 'https://github.com/user/project-three'
        }
      ]
    };
  }
};
</script>

<style scoped>
.projects-container {
  padding: 20px;
  background: #e0e0e0; /* Example background for neumorphism */
  border-radius: 20px;
  box-shadow: 8px 8px 20px #b8b8b8, 
              -8px -8px 20px #ffffff;
}

.project {
  margin: 15px 0;
  padding: 15px;
  background: #f0f0f0; /* Example project card background */
  border-radius: 15px;
  box-shadow: 5px 5px 15px #b8b8b8, 
              -5px -5px 15px #ffffff;
}

.project h3 {
  margin: 0;
}

.project a {
  color: #007bff;
  text-decoration: none;
}
</style>