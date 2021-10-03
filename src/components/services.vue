<template>
<!-- PARENT DIV -->
  <div class="container-fluid col-lg-12 ml-4">
    <!-- ROW -->
    <div class="row ml-3">
      <!-- COLUMN -->
      <div class="col-lg-12 modules rounded bg-white p-4 pb-5">
        <!-- ICON -->
        <p class="orange-color font-30"><i :class="moduleData.icon"></i></p>
        <!-- TITLE -->
        <span class="text-black bebas-30">{{ moduleData.title }}</span><br>
        <!-- DESCRIPTION -->
        <span class="grey-color"> {{ moduleData.description}} </span>
    </div> <!-- END OF COLUMN -->
    </div> <!-- END OF ROW -->
  </div> <!-- END OF PARENT DIV -->
</template>

<script>
export default {
  name: 'services',
  props: ['moduleData']
}
</script>

<style scoped>
.modules {
  width: 300px;
  border: 1px solid #c5c4c4;
}

.modules:hover {
  border: 1px solid #f78503;
}

.font-30 {
  font-size: 30px;
}
</style>
