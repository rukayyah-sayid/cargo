<template>
  <div class="container-fluid ml-4 mb-4">
    <div class="row mt-4">
      <div class="col-lg-12 ml-2">
        <div class="card modules border-black rounded justify-content-center p-4">
          <span class="bebas-30 text-center mt-3"> {{ prices.title }} </span>
          <span class="dm-sans-50 font-weight-bold orange-color text-center"> {{ prices.price }} <span class="dm-sans-18 font-weight-normal grey-color">/ {{ prices.period }} </span></span>
          <ul class="list-unstyled mt-3">
            <li class="grey-color dm-sans-14"> <i class="fas fa-check orange-color pb-3"></i> &nbsp; {{ prices.options[0] }} </li>
            <li class="grey-color dm-sans-14"> <i class="fas fa-check orange-color pb-3"></i> &nbsp; {{ prices.options[1] }} </li>
            <li class="grey-color dm-sans-14"> <i class="fas fa-check orange-color pb-3"></i> &nbsp; {{ prices.options[2] }} </li>
            <li class="grey-color dm-sans-14"> <i class="fas fa-check orange-color pb-3"></i> &nbsp; {{ prices.options[3] }} </li>
            <li class="grey-color dm-sans-14"> <i class="fas fa-check orange-color pb-3"></i> &nbsp; {{ prices.options[4] }} </li>
          </ul>
          <div class="mx-auto col-lg-4 pb-4 pt-3">
            <button type="button" class="btn btn-buy orange-background dm-sans-14 text-white"> Buy Now </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'pricing',
  props: ['prices']
}
</script>

<style scoped>
.btn-buy {
  margin-left: -15px;
}
</style>
