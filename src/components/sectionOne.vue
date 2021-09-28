<template>
  <!-- SECTION 1 -->
    <div class="section-1 container-fluid">
      <div class="text col-5 pl-5 ml-5">
        <span class="font-weight-bold text-white dm-sans-36 mt-5">CHOOSE YOUR QUALITY DELIVERY OF YOUR CARGO</span>
        <div class="input-group mt-4">
          <div class="form-outline m-0 p-0 col-lg-10">
            <input type="search" placeholder="Enter your tracking number" class="form-control pt-3 pb-3 " />
          </div>
          <div>
            <button type="button" class="btn search-btn p-3">
              <i class="fas fa-search"></i>
            </button>
          </div>
        </div>
      </div>
    </div>
    <!-- SECTION 1 END -->
</template>

<script>
export default {
  name: 'sectionOne'
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans&display=swap');

/* SECTION-1 */
.section-1 {
  background-image: url("../assets/background.png");
  /* width: 1366px; */
  height: 500px;
  
}

.text {
  padding-top: 150px;
}

::placeholder {
  font-family: 'DM Sans', sans-serif;
  font-size: 18px;
}

input[type=search] {
  width: 403px;
}

.search-btn {
  color: white;
  background: #f78503;
}

</style>
