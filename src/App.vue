<template>
  <!-- PARENT CONTAINER -->
  <div class="container-fluid m-0 p-0">
    <!-- NAVBAR -->
    <navbar/>
    <!-- FIRST SECTION -->
    <sectionOne/>
    <!-- SERVICES -->
    <div class="grey-background pt-5 pb-5 col-lg-12" id="services">
      <div class="col-lg-6 mx-auto mt-5">
        <h2 class="bebas-50 text-center orange-color">WHAT WE OFFER</h2>
      <h6 class="grey-color dm-sans-18 text-center">Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.</h6>
      </div>
    <div class="row ml-5 pl-5">
      <div v-for="category in categories" :key="category.title" class="pt-5">
        <services :moduleData = "category"></services>
      </div>
    </div>
    </div> <!-- END OF SERVICES -->
    <!-- ABOUT US -->
    <div class="col-lg-12 pb-5">
      <div class="col-lg-6 mx-auto mt-5">
        <h2 class="bebas-50 orange-color text-center pt-5">About Us</h2>
        <p class="grey-color dm-sans-18 text-center">Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.</p>
      </div>
      
      <div class="row ml-5 pl-5 mt-5">
        <div v-for="data in statistics" :key="data.rate" class="row">
        <about-us :statistics-data="data" class="mr-5"/>
      </div>
      </div>
    </div> <!-- END OF ABOUT US -->
    <!-- OUR STAFF -->
    <div class="grey-background col-lg-12 pb-5">
      <div class="col-lg-6 mx-auto mt-5 pt-5">
        <h2 class="bebas-50 orange-color text-center pt-5">our staff</h2>
        <p class="grey-color dm-sans-18 text-center">Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.</p>
      </div>

      <div class="row ml-5 pl-5 mt-5">
        <div v-for="info in staff" :key="info.image" class="row">
        <our-staff :details="info" class="mr-"/>
      </div>
      </div>
    </div>
    <!-- END OF OUR STAFF -->
    <!-- PRICING -->
    <div class="col-lg-12 pb-5">
      <div class="col-lg-6 mx-auto mt-5">
        <h2 class="bebas-50 orange-color text-center pt-5">PRICING</h2>
        <p class="grey-color dm-sans-18 text-center">Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.</p>
      </div>
      
      <div class="row ml-5 pl-5 mt-5">
        <div v-for="price in pricing" :key="price.title" class="row">
        <pricing :prices="price" class="mr-"/>
      </div>
      </div>
    </div> <!-- END OF PRICING -->
    </div> <!-- END OF PARENT CONTAINER -->
</template>

<script>
import navbar from './components/navbar.vue'
import sectionOne from './components/sectionOne.vue'
import services from './components/services.vue'
import aboutUs from './components/aboutUs.vue'
import ourStaff from './components/ourStaff.vue'
import pricing from './components/pricing.vue'

export default {
  name: 'App',
  components: {
    navbar,
    sectionOne,
    services,
    aboutUs,
    ourStaff,
    pricing
    },

    data() {
      return {
        categories: [
          {
            icon: 'fad fa-ship',
            title: 'SEA FREIGHT',
            description: 'A small river named Duden flows by their place and supplies it with the necessary regelialia.'
          },
          {
            icon: 'fas fa-plane',
            title: 'AIR FREIGHT',
            description: 'A small river named Duden flows by their place and supplies it with the necessary regelialia.'
          },
          {
            icon: 'fas fa-shopping-cart',
            title: 'PACKAGE FOWARDING',
            description: 'A small river named Duden flows by their place and supplies it with the necessary regelialia.'
          },
          {
            icon: 'fas fa-truck',
            title: 'TRUCKING',
            description: 'A small river named Duden flows by their place and supplies it with the necessary regelialia.'
          },
          {
            icon: 'fas fa-warehouse',
            title: 'WAREHOUSE',
            description: 'A small river named Duden flows by their place and supplies it with the necessary regelialia.'
          },
          {
            icon: 'fas fa-save',
            title: 'DELIVERY',
            description: 'A small river named Duden flows by their place and supplies it with the necessary regelialia.'
          }
        ],

        statistics: [
          {
            rate: "500+",
            text: "Years of Experience"
          },
          {
            rate: "300+",
            text: "Companies"
          },
          {
            rate: "108+",
            text: "Covered Countries"
          },
          {
            rate: "1,500+",
            text: "Couriers"
          }
        ],

        staff: [
          {
            image: '../assets/image1.jpg',
            name: 'Ikram Sayid',
            role: 'CEO',
            bio: 'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.'
          },
          {
            image: '../assets/image2.jpg',
            name: 'Hauwa Dalhatu',
            role: 'PROJECT MANAGER',
            bio: 'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.'
          },
          {
            image: '../assets/image3.png',
            name: 'Zulaikha Abubakar',
            role: 'UI DESIGNER',
            bio: 'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.'
          },
          {
            image: '../assets/image4.jpg',
            name: 'Samah Mustapha',
            role: 'ACCOUNTANT',
            bio: 'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.'
          },
          {
            image: '../assets/image5.jpg',
            name: 'Huda Kamal',
            role: 'AUDITOR',
            bio: 'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.'
          },
          {
            image: '../assets/image6.jpg',
            name: 'Rayyan Ahmad',
            role: 'VENDOR',
            bio: 'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.'
          }
        ],
        pricing: [
          {
            title: 'basic',
            price: '$200',
            period: 'annum',
            options: [
              'Officia quaerat eaque neque',
              'Possimus aut consequuntur incidunt',
              'Lorem ipsum dolor sit amet',
              'Consectetur adipisicing elit',
              'Dolorum esse odio quas architecto sint'
            ]
          },

          {
            title: 'Premium',
            price: '$600',
            period: 'annum',
            options: [
              'Officia quaerat eaque neque',
              'Possimus aut consequuntur incidunt',
              'Lorem ipsum dolor sit amet',
              'Consectetur adipisicing elit',
              'Dolorum esse odio quas architecto sint'
            ]
          },

          {
            title: 'professional',
            price: '$800',
            period: 'annum',
            options: [
              'Officia quaerat eaque neque',
              'Possimus aut consequuntur incidunt',
              'Lorem ipsum dolor sit amet',
              'Consectetur adipisicing elit',
              'Dolorum esse odio quas architecto sint'
            ]
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
.dm-sans-12 {
  font-family: 'DM Sans', sans-serif;
  font-size: 12px;
}

.dm-sans-14 {
  font-family: 'DM Sans', sans-serif;
  font-size: 14px;
  line-height: 30px;
}

.dm-sans-18 {
  font-family: 'DM Sans', sans-serif;
  font-size: 18px;
  line-height: 30px;
}

.dm-sans-36 {
  font-family: 'DM Sans', sans-serif;
  font-size: 36px;
}

.dm-sans-50 {
  font-family: 'DM Sans', sans-serif;
  font-size: 50px;
}

.bebas-20 {
  font-family: 'Bebas Neue', cursive;
  font-size: 20px;
}

.bebas-30 {
  font-family: 'Bebas Neue', cursive;
  font-size: 30px;
}

.bebas-50 {
  font-family: 'Bebas Neue', cursive;
  font-size: 50px;
}

.orange-color {
  color: #f78503;
}

.orange-background {
  background: #f78503;
} 

.grey-color {
  color: rgb(109, 107, 107);
}

.grey-background {
  background: rgb(238, 236, 236);
}
</style>
