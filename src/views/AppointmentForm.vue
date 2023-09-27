<template>
    <form class="appointment-form">
      <h2>Book an Appointment with Us</h2>
      <img src="carappointment.jpeg" alt="Appointment Image" class="appointment-image" />
      <div class="form-group">
        <label for="name">Name:</label>
        <input type="text" id="name" v-model="name" required />
      </div>
      <div class="form-group">
        <label for="phone">Phone:</label>
        <input type="tel" id="phone" v-model="phone" required />
      </div>
      <div class="form-group">
        <label for="appointment-time">Appointment Time:</label>
        <input type="datetime-local" id="appointment-time" v-model="appointmentTime" required />
      </div>
      <button type="submit">Submit</button>
    </form>
  </template>
  
  <script>
  export default {
    data() {
      return {
        name: '',
        phone: '',
        appointmentTime: '',
      };
    },
  };
  </script>
  
  <style scoped>
  .appointment-form {
    text-align: center;
    padding: 20px;
  }
  
  h2 {
    font-size: 24px;
  }
  
  .appointment-image {
    max-width: 100%;
    height: auto;
    margin: 20px 0;
  }
  
  .form-group {
    margin: 10px 0;
  }
  
  label {
    font-weight: bold;
  }
  
  input[type="text"],
  input[type="tel"],
  input[type="datetime-local"] {
    width: 100%;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
  }
  </style>
  