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
          'Host': 'https://3ytvvyi4.directus.app'
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
          <ul v-for=" (item, index) in items.data.translations" :key="index">
            <li > {{item.body}} </li> 
            <!-- <li>{{ item }}</li> -->
          </ul>
        </div>
      </div>
    </div>

  </div>


</template>

<style scoped>

</style>