<script setup>
defineProps({
  herocont: []
})
</script>


<template>
  <img :src="herocont.herobg">
  <div class="inner-container">
    <img :src="herocont.imageurl" alt="">
    <div class="content">
      <div class="content-block">
        <div>
          <h2>{{ herocont.title }}</h2>
          <p>{{ herocont.contentBlocks[0].discription }}</p>
          <!-- <div v-for="bob in herocont.contentBlocks[0] ">  -->



          <div :data-content="JSON.stringify(contentBlock)" v-for="contentBlock in herocont.contentBlocks"> {{ JSON.stringify(bob) }}{{ bob }}

            <div :data-smH="JSON.stringify(smH)" v-for="smH in contentBlock.sub_moduleHotspot">

              <!-- <pre>{{JSON.stringify(rob)}}</pre> -->
              <a :data-button="JSON.stringify(button)" v-for="button in smH.buttonlist" :href="button.url" :class="button.type">
                <!-- {{JSON.stringify(shawn)}} -->
                <span>{{ button.text }}</span>
              </a>

            </div>



          </div>
          <!-- <div v-for="rob in bob">
            {{ rob }}
          </div> -->
          <!-- </div> -->
          <!-- <div >{{herocont.contentBlocks.sub_moduleHotspot}}</div> -->
          <!-- <div class="svg-btn-grid">
            <img v-for=" heroimg, index in herocont.contentBlocks[0].sub_moduleHotspot" :key="index" :src="heroimg.icnurl" alt="">
          </div>
          <div v-for=" bob, index in herocont.sub_modulesHotspot " :key="index">
            <a href=""> {{ bob }}</a>
            <pre>{{ bob }}</pre>
          </div> -->
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
/* .content-block {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 100px;
} */



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