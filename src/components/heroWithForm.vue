<script setup>
defineProps({
  herocont: []
})
</script>


<template>

  <div class="heroBannerContainer">
    <img :src="herocont.bgImage" :alt="wee" class="image">
    <div class="overlay">
      <img :src="herocont.bgImageOverlay" :alt="wee" class="overlayImage">
    </div>
  </div>

  <div class="inner-container">
    <div class="content">
      <div class="content-block">
        <div class="content-half">
          <div>
            <img v-for="logo in herocont.brandLogoList" :src="logo.url" :alt="logo.alt">
            <h2>{{ herocont.title }}</h2>+-
            <p>{{ herocont.description }}</p>
            <span>
              <a href="">
                <img src="" alt="">
              </a>
            </span>
          </div>
          <img v-for="image in herocont.imageList" :src="image.imageurl" alt="">
        </div>

        <div class="content-half">
          <div>
            <ul>
              <h3></h3>
              <li></li>
            </ul>    
          </div>
        </div>
      </div>
    </div>
  </div>
</template>



<style scoped>

</style>