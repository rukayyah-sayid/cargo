<template>
<div class="container-fluid ml-4 mb-">
    <div class="row mt-4 pt-">
      <div class="col-lg-12 ml-3">
        <div class="card modules border-black rounded justify-content-center p-4">
          <img :src="details.image" width="120" height="120" class="rounded mx-auto circle img mt-3 mb-3" alt="">
          <span class="bebas-20 text-center mt-3"> {{ details.name }} </span>
          <span class="dm-sans-12 grey-color text-center"> {{ details.role }} </span>
          <p class="dm-sans-12 mt-3 text-center"> {{ details.bio }} </p>

          <div class="row col-lg-4 m-0 p-0 mx-auto mb-3">
            <div class="col m-0 p-0"><i class="fab fa-twitter-square orange-color font-25"></i></div>
            <div class="col m-0 p-0"><i class="fab fa-facebook-square orange-color font-25"></i></div>
            <div class="col m-0 p-0"><i class="fab fa-snapchat-square orange-color font-25"></i></div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!-- <div class="card border-black col-lg-12 rounded justify-content-center">
    <img :src="details.image" width="50" height="50" class="rounded circle img" alt="">
    <p class="bebas-20 text-center"> {{ details.name }} </p>
  </div> -->
</template>

<script>
export default {
  name: 'ourStaff',
  props: ['details']
}
</script>

<style scoped>

.modules {
  width: 320px;
  border: 1px solid #c5c4c4;
}

.font-25 {
  font-size: 25px;
}

/* .modules:hover {
  border: 1px solid #f78503;
} */

</style>
