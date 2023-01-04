<script setup>
defineProps({
  navbtn: []
})
// export default {
  //   props: {
    //     navbtn: []
    
    //   }
    // }
    
    
  </script>
  
<template>
    <div class="container">
      <figure class="logo menu-item" itemprop="logo" itemscope itemtype="https://schema.org/ImageObject">
        <a class="img" href="/" aria-current="page">
          <span>
            Go To Home
          </span>
          <img itemprop="thumbnail" src="\src\assets\BuyChain-Logo-REV.svg" width="141" height="51"
          alt="Go To Home" />
        </a>
        <figcaption itemprop="caption"></figcaption>
      </figure>
      <ul class = "main-nav-links">
        <li v-for="(options, index) in navbtn" :key="index">
          <a class="" :href="options.url">{{ options.label }}</a>
        </li>
      </ul>
    </div>
  </template>
  
<style scoped>
.main-nav-links {
    margin-right:0;
    width: 100%;
    text-align: right;
  }
  .main-nav-links a {
    font-weight:var(--fw-bold);
    transition:300ms;
    position:relative;
  }
  .main-nav-links a::after {
    content:"";
    display:block;
    position:absolute;
    height:4px;
    background:var(--accent-light);
    width:0px;
    bottom:0;
    left:0;
    transition:500ms;
  }
  .main-nav-links li a:hover {
    color:  var(--secondary-light);
  }
  .main-nav-links li a:hover::after {
    width:100%;
    transition:500ms;
    height:4px;
  }
  .img>span {
    display: none;
  }
  
  figure {
    margin: unset;
    margin-top: auto;
    margin-bottom: auto;
    
  }
  
  img {
    max-width: 100%;
    height: auto;
    vertical-align: middle;
  }
  
  ul {
    margin: unset;
  }
  
  li {
    display: inline;
    color: var(--bg-layer-100);
    padding-right: 20px ;
  }
  
  li:last-child {
    color: var(--head-text-color);
    background-color: var(--btn-1-background-color);
    border: 2px solid var(--btn-1-background-color);
    border-radius: 5px;
    padding: 0.3em 0.6em;
    margin: 0.3em 0 0.3em 0.3em;
    
  }
  
  
  nav {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    height: fit-content;
    padding: 12px 0;
  }
</style>