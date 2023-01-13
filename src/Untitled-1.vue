<script lang="ts">

export default {
  data() {
    return {
      items: []
    };
  },
  methods: {
    fetchItems() {
      const options = {
        method: 'GET',
        headers: {
          'Authorization': 'Bearer xUu7uNUFtkVRl3uwpeMvZngHUvf1MOT4',
          'Host': 'https://3ytvvyi4.directus.app/'
        }
      };

      fetch('https://3ytvvyi4.directus.app/items/articles/10?fields[]=translations.body', options)
        .then(response => response.json())
        .then((data) => (this.items = data));
      console.log(this);
    }
  },
  mounted() {
    this.fetchItems();
  }
};
console.log(this);
</script>



<template>
  <div class="container">
    <div class="inner-container">
      <div class="content">
        <div class="content-block">
          <!-- <div>
            <h1>{{items}}</h1>
            <p></p>
          </div> -->
          <!-- <span>{{ JSON.stringify(items.data.translations[0].body[0]) }}</span> -->
          <ul>
            <!-- <li v-for="item in items.keys(translations)"> -->
              <!-- <span>{{ item }}</span></li> -->
            <!-- <li :data-div="item,never)" v-for=" (item, index) in items" :key="index" > -->
              <!-- <span v-for="piece in item.translations"></span> {{piece}} </li> -->
            <!-- <li>{{ item }}</li> -->
        <!-- </li>   -->
        </ul>
        </div>
      </div>
    </div>
  </div>


</template>

<style scoped>

</style>