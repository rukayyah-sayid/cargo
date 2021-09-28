<template>
  <div class="navbar navbar-expand-sm mt-4 mb-2 fixed-top navbar-transparent dm-sans-18">
      <!-- LINKS -->
        <ul class="navbar-nav">
          <li class="nav-item">
            <img class="mr-5" src="../assets/LOGO1.png" width="150" alt="">
          </li>
          <li class="nav-item ml-5 pl-5">
            <a href="#" class="navbar-link mr-5">Home</a>
          </li>
          <li class="nav-item">
            <a href="#" class="navbar-link mr-5">Services</a>
          </li>
          <li class="nav-item">
            <a href="#" class="navbar-link mr-5">About</a>
          </li>
          <li class="list-inline list-item">
            <a href="#" class="navbar-link mr-5">Why Us</a>
          </li>
          <li class="list-inline list-item">
            <a href="#" class="navbar-link mr-5">Testimonials</a>
          </li>
          <li class="list-inline list-item">
            <a href="#" class="navbar-link mr-5">Blog</a>
          </li>
          <li class="list-inline list-item">
            <a href="#" class="navbar-link mr-5">Contact</a>
          </li>
        </ul> <!-- LINKS END -->
      </div>
</template>

<script>
export default {
  name: 'navbar',
  props: {},
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans&display=swap');

.navbar-nav {
  margin-left: -80px;
}

.navbar-link {
  color: white;
}

.navbar-link:hover {
  text-decoration: none !important;
  color: white;
}

.navbar-link:focus {
  color: #f78503;
  font-weight: bold;
  text-decoration: none;
}

</style>
