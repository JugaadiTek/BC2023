<script setup>
defineProps({
  herocont: []
})
</script>


<template>
      <div class="inner-container">
        <div class="content">
          <div class="content-block">

            <div>
              <h2>{{ herocont.title }}</h2>
              <p>{{ herocont.discription }}</p>
              <img v-for= " heroimg, index in herocont.iconurl" :key="index" :src="heroimg.icnurl" alt="">
            </div>
            <img :src="herocont.imageurl" alt="">
            <div v-for=" bob , index in herocont.sub_modulesHotspot " :key="index">
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

.content-block>div>img {
  height: 175px;

}
@media (max-width: 600px) {
  .content-block {
    grid-template-columns: repeat(1, 1fr);
  }
}


</style>