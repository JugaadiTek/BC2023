<script setup>
defineProps({
  herocont: []
})
</script>


<template>
  <img :src="herocont.herobg">
  <div class="inner-container">
    <div class="content">
      <div class="content-block">
        <div>
          <h2>{{ herocont.title }}</h2>
          <p>{{ herocont.discription }}</p>
          <div class="svg-btn-grid">
            <img v-for=" heroimg, index in herocont.iconurl" :key="index" :src="heroimg.icnurl" alt="">
          </div>
        </div>
        <img :src="herocont.imageurl" alt="">
        <div v-for=" bob, index in herocont.sub_modulesHotspot " :key="index">
          <a href=""> {{ bob }}</a>
          <pre>{{ bob }}</pre>
        </div>
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

section.hero>div>img {
  position: absolute;
  width: 100%;
  z-index: -1;
  top: 100%;
  left: 100%;
  transform: translate(-100%, -100%);
}
</style>