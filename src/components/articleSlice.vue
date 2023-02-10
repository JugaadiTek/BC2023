<script setup>
defineProps({
  articleSliceCont: []
})
</script>

<template>
  <div class="inner-container">
    <div class="content">
      <!-- <div class="articleTags">
        <ul>
          <li v-for="tag in tags"> 
            <a :href="tag.tagLink" class="tagbutton">{{ tag.tagText }}</a>
          </li>
        </ul>
      </div> -->
      <div class="content-block">
        <div>
          <article class="articleColumn">
            {{ articleSliceCont.wysiwyg }}
          </article>
          <!-- <article v-for="paragraph in paragraphs">
            {{ paragraph }}
          </article> -->
          <aside class="authorColumn">
            <img class="authorImage" src="" alt="">
            <div class="authorInfo">
              <h3>{{ authorName }}</h3>
              <p>{{ authorTitle }}</p>
              <p>{{ authorBio }}</p>
            </div>
            <div class="authorSocialLinks">
              <ul>
                <li v-for="socialLink in socialLinks">
                  <a :class="socialLink.socialLinkClass" :href="socialLink.socialLinkUrl">
                    {{ socialLink.socialLinkText }}
                  </a>
                </li>
              </ul>
            </div>
            <div class="articlesByAuthor">
              <h4>More Articles by {{ authorName }}</h4>
              <ul>
                <li v-for="article in articles">
                  <a :href="articleLink">{{ articleTitle }}</a>
                </li>
              </ul>
            </div>
            <span>
              <!-- <a class=" button type_01" :href="">Previous</a> -->
              <!-- <a class=" button type_02" :href="">Load More</a> -->
              <!-- <a class=" button type_01" :href="">Next</a> -->
            </span>
          </aside>
        </div>
        
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