<template>
  <div class="container-fluid">
    <div class="row mx-auto ml-5 pl-5">
      <div class="col-lg-12 ml-3">
        <p class="orange-color font-weight-bold dm-sans dm-sans-50"> {{ statisticsData.rate }} </p>
        <div class="bottom-border mx-auto"></div>
        <p class="grey-color dm-sans-12 font-weight-bold text-center mt-2"> {{ statisticsData.text }} </p>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'aboutUs',
  props: ['statisticsData']
}
</script>

<style scoped>

.bottom-border {
  border-bottom: 2px solid grey;
  width: 70px;
}

</style>
