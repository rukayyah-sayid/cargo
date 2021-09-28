<template>
  <div class="container-fluid col-lg-12">
    <div class="row">
      <div class="col-lg-3 border">
      <ul class="list-unstyled">
        <!-- <li> {{ moduleData.icon }} </li> -->
        <li class="text-black bebas-30"> {{ moduleData.title }} </li>
        <li class="grey-color text-justify"> {{ moduleData.description }} </li>
      </ul>
    </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['moduleData']
}
</script>

<style scoped>

</style>
