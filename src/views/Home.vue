<template>
  <div class="home">
    <div class="header">
      <h1>Welcome to Cheap Car Rentals</h1>
      <p>Your trusted partner for affordable and reliable car rentals.</p>
      <img src="contact.jpeg" alt="Cheap Car Rentals Logo" height="400" width="600" />
    </div>
    <nav>
      <router-link to="/rent">Rent a Car</router-link>
      <router-link to="/appointment">Book an Appointment</router-link>
      <router-link to="/contact">Contact Us</router-link>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Home',
};
</script>

<style scoped>
.home {
  text-align: center;
  padding: 20px;
}

.header {
  background-color: #007BFF;
  color: #fff;
  padding: 20px;
  border-radius: 5px;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
}

.logo {
  max-width: 100px;
  margin-bottom: 20px;
}

h1 {
  font-size: 36px;
  margin: 0;
  padding-top: 10px;
}

nav {
  margin-top: 20px;
}

nav a {
  margin: 0 10px;
  text-decoration: none;
  font-size: 18px;
  color: #007BFF;
  transition: color 0.3s;
}

nav a:hover {
  color: #0056b3;
}
.header p {
  font-size: 18px;
  margin-top: 10px;
  color: #fff;
}
</style>
