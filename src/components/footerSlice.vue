<script setup>
defineProps ({
  footerCont:[]
})
</script>


<template>
<div class="container">
  <div class="inner-container">
    <div class="content">
      <div class="content-block">
        <div>
          <span></span>
          <span></span>
        </div>
        <div>
          <ul>
            <li v-for="link in link_list" ></li>
          </ul>
          <ul>
            <li></li>
          </ul>
          <ul>
            <li></li>
          </ul>
          <ul>
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