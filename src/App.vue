<template>
  <div class="container-fluid m-0 p-0">
    <navbar/>
    <sectionOne/>
    <div class="grey-background pt-3 col-lg-12">
      <h2 class="bebas-60 orange-color text-center pt-5">WHAT WE OFFER</h2>
      <div v-for="category in categories" :key="category.title">
        <services :moduleData = "category"></services>
      </div>
    </div>
    </div>
</template>

<script>
import navbar from './components/navbar.vue'
import sectionOne from './components/sectionOne.vue'
import services from './components/services.vue'

export default {
  name: 'App',
  components: {
    navbar,
    sectionOne,
    services
    },

    data() {
      return {
        categories: [
          {
            // icon: '',
            title: 'SEA FREIGHT',
            description: 'A small river named Duden flows by their place and supplies it with the necessary regelialia.'
          },
          {
            // icon: '',
            title: 'AIR FREIGHT',
            description: 'A small river named Duden flows by their place and supplies it with the necessary regelialia.'
          },
          {
            // icon: '',
            title: 'PACKAGE FOWARDING',
            description: 'A small river named Duden flows by their place and supplies it with the necessary regelialia.'
          },
          {
            // icon: '',
            title: 'TRUCKING',
            description: 'A small river named Duden flows by their place and supplies it with the necessary regelialia.'
          },
          {
            // icon: '',
            title: 'WAREHOUSE',
            description: 'A small river named Duden flows by their place and supplies it with the necessary regelialia.'
          },
          {
            // icon: '',
            title: 'DELIVERY',
            description: 'A small river named Duden flows by their place and supplies it with the necessary regelialia.'
          }
        ]
      }
    }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap');

/* FONTS */
.dm-sans-18 {
  font-family: 'DM Sans', sans-serif;
  font-size: 18px;
}

.dm-sans-36 {
  font-family: 'DM Sans', sans-serif;
  font-size: 36px;
}

.bebas-30 {
  font-family: 'Bebas Neue', cursive;
  font-size: 30px;
}

.bebas-60 {
  font-family: 'Bebas Neue', cursive;
  font-size: 60px;
}

.orange-color {
  color: #ff5722;
  /* background: #ff5722; */
}

.grey-color {
  color: rgb(109, 107, 107);
}

.grey-background {
  background: rgb(243, 241, 241);
}
</style>
