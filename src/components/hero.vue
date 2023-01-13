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
        <div>
          <!-- <img v-for="logo in herocont.brandLogoList" :src="logo.url" :alt="logo.alt"> -->
          <h2>{{ herocont.title }}</h2>
          <p>{{ herocont.description }}</p>
          <!-- <span >
            <a v-for="(atom, index) in herocont.atoms" :key="index" :href="atom.url">{{atom.text}}</a>
          </span> -->
        </div>
        <img v-for="image in herocont.imageList" :src="image.imageurl" alt="">

      </div>
    </div>
  </div>
</template>

<style scoped>

.content-block {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 100px;
}

@media (max-width: 600px) {
  .content-block {
    grid-template-columns: repeat(1, 1fr);
  }
}

section.hero {
  background-size: cover;
  background-repeat: no-repeat;
  overflow: hidden;
  margin-bottom: 64px;
  position: relative;
}

/* section.hero>div>div>img, section.hero>div>div>div>img {
  position: absolute;
  width: 100%;
  z-index: -1;
  top: 100%;
  left: 100%;
  transform: translate(-100%, -100%);
} */



/* parallax effect hero banner */
.heroBannerContainer {
  position: relative;
}

.image {
  display: block;
  width: 100%;
  height: auto;
  opacity: 50%;
  filter: blur(1px);
  -webkit-filter: blur(1px);
  position: absolute;
  z-index: -1;
  top: 100%;
  left: 100%;
  transform: translate(-100%, -100%);
}

.overlay {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0;
  transition: .7s ease;
}

.heroBannerContainer:hover .overlay {
  opacity: 1;
}

.overlayImage {
  position: absolute;
  width: 100%;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
}
</style>