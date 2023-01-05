<script setup>
defineProps({
  artcontent: []
})
</script>


<template>
      <div class="inner-container">
        <div class="content">
          <div class="content-block">
            <h2>{{ artcontent.tittle }}</h2>
            <p> {{ artcontent.discription }} </p>

            <div v-for="guddu in artcontent.boxycontent">

              <img :src="guddu.imgurl" alt="" height="220" width="370">


              <div>
                <h3>{{ guddu.tittle }}</h3>
                <p> {{ guddu.details }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
</template>

<style scoped>

.content-block>div {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 100px;
  margin: 50px 0px;
  text-align: left;
  align-self: center;
  /* overflow: hidden; */
  padding: 10px ;
}

img {
  border-radius: 6px;
  border: 10px solid #ffffff;
  box-shadow: 0px 1px 5px;
  width: 100%;
  height: 100%;
}

@media (max-width: 600px) {
  .content-block>div {
    grid-template-columns: repeat(1, 1fr);
  }
}

@media (max-width: 400px) {
  .content-block>div {
    grid-template-columns: repeat(1, 1fr);
  }
}
</style>