<script setup>
defineProps({
  articleSliceCont: []
})
</script>


<template>
  <div class="inner-container">
    <div class="content">
      <div class="articleTags">
        <ul>
          <li> <a href="">{{ articleTag }}</a>
          </li>
        </ul>
      </div>
      <div class="content-block">
        <div>
          <article class="articleColumn">
            {{ articleSliceCont.wysiwyg }}
          </article>
          <aside class="authorColumn">
            <img class="authorImage" src="" alt="">
            <div class="authorInfo">
              <h3>{{ authorName }}</h3>
              <p>{{ authorTitle }}</p>
              <p>{{ authorBio }}</p>
            </div>
            <div class="authorSocialLinks">
              <a href="">Twitter</a>
              <a href="">LinkedIn</a>
              <a href="">E-mail</a>
            </div>
            <div class="articlesByAuthor">
              <h3>More Articles by {{ authorName }}</h3>
              <ul>
                <li>
                  <a href="">Article Title</a>
                </li>
              </ul>
            </div>
          </aside>
        </div>
        <span>
          <a class=" button type_01" href="">Previous</a>
          <a class=" button type_02" href="">Load More</a>
          <a class=" button type_01" href="">Next</a>
        </span>
      </div>
    </div>
  </div>
</template>



 
<style scoped>
.content-block > div {
  display: grid;
  grid-template-columns: 2fr 1fr;
}

.content-block {
  text-align: center;
}

span > a {
  display: inline-block;
  margin: 0 40px;
  padding: 5px 10px;
  width: 200px;
}
</style>