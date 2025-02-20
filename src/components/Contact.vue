<template>
  <div class="contact-container">
    <h2>Contact Me</h2>
    <form @submit.prevent="submitForm">
      <div class="form-group">
        <label for="name">Name:</label>
        <input type="text" id="name" v-model="name" required />
      </div>
      <div class="form-group">
        <label for="email">Email:</label>
        <input type="email" id="email" v-model="email" required />
      </div>
      <div class="form-group">
        <label for="message">Message:</label>
        <textarea id="message" v-model="message" required></textarea>
      </div>
      <button type="submit">Send Message</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: '',
      email: '',
      message: ''
    };
  },
  methods: {
    submitForm() {
      // Handle form submission logic here
      console.log('Form submitted:', this.name, this.email, this.message);
      // Reset form fields
      this.name = '';
      this.email = '';
      this.message = '';
    }
  }
};
</script>

<style scoped>
.contact-container {
  background: #e0e0e0;
  border-radius: 20px;
  box-shadow: 10px 10px 20px #b0b0b0, -10px -10px 20px #ffffff;
  padding: 20px;
  max-width: 400px;
  margin: auto;
}

.form-group {
  margin-bottom: 15px;
}

input, textarea {
  width: 100%;
  padding: 10px;
  border: none;
  border-radius: 10px;
  box-shadow: inset 5px 5px 10px #b0b0b0, inset -5px -5px 10px #ffffff;
}

button {
  background: #ffffff;
  border: none;
  border-radius: 10px;
  padding: 10px 15px;
  cursor: pointer;
  box-shadow: 5px 5px 10px #b0b0b0, -5px -5px 10px #ffffff;
}
</style>