<template>

  <div class="heroBannerContainer">
    <img src="src\assets\AdobeStock_524865233.jpeg" alt="travel" class="image">
    <div class="overlay">
      <img src="src\assets\8562956_25550 [Converted].svg" alt="" class="overlayImage zoom">
    </div>
  </div>
</template>

<style scoped>
.heroBannerContainer {
  position: relative;
}

.image {
  display: block;
  width: 100%;
  height: auto;
  opacity: 50%;
  filter: blur(1px);
  /* -webkit-filter: blur(1px); */
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
  color: white;
  font-size: 18px;
  position: absolute;
  width: 100%;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
}

</style>