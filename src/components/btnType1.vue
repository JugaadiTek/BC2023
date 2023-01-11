<script setup>

</script>

<template>
 <button class="button-85 " role="button">Button 85</button>
</template>


<style scoped>
.button-85 {
 padding: 0.6em 2em;
 border: none;
 outline: none;
 color: rgb(255, 255, 255);
 background: #111;
 cursor: pointer;
 position: relative;
 z-index: 0;
 border-radius: 10px;
 user-select: none;
 -webkit-user-select: none;
 touch-action: manipulation;
}

.button-85:before {
 content: "";
 background: linear-gradient(45deg,
 var(--brand-white),
     
 var(--secondary),
 var(--brand-white),
 var(--accent),
var(--brand-white) );
 position: absolute;
 top: -2px;
 left: -2px;
 background-size: 400%;
 z-index: -1;
 filter: blur(5px);
 -webkit-filter: blur(5px);
 width: calc(100% + 4px);
 height: calc(100% + 4px);
 animation: glowing-button-85 20s linear infinite;
 transition: opacity 0.3s ease-in-out;
 border-radius: 10px;
}

@keyframes glowing-button-85 {
 0% {
   background-position: 0 0;
 }

 50% {
   background-position: 400% 0;
 }

 100% {
   background-position: 0 0;
 }
}

.button-85:after {
 z-index: -1;
 content: "";
 position: absolute;
 width: 100%;
 height: 100%;
 /* background: var(--secondary); */
 background: black;
 left: 0;
 top: 0;
 border-radius: 10px;
}
</style>
















<!-- another button type with neon shodow effect -->
<!-- 
  <template>

<button class="button-62" role="button">Button 62</button>

</template>


<style scoped>
.button-62 {
 background: linear-gradient(to bottom right, #EF4765, #FF9A5A);
 border: 0;
 border-radius: 12px;
 color: #FFFFFF;
 cursor: pointer;
 display: inline-block;
 font-family: -apple-system,system-ui,"Segoe UI",Roboto,Helvetica,Arial,sans-serif;
 font-size: 16px;
 font-weight: 500;
 line-height: 2.5;
 outline: transparent;
 padding: 0 1rem;
 text-align: center;
 text-decoration: none;
 transition: box-shadow .2s ease-in-out;
 user-select: none;
 -webkit-user-select: none;
 touch-action: manipulation;
 white-space: nowrap;
}

.button-62:not([disabled]):focus {
 box-shadow: 0 0 .25rem rgba(0, 0, 0, 0.5), -.125rem -.125rem 1rem rgba(239, 71, 101, 0.5), .125rem .125rem 1rem rgba(255, 154, 90, 0.5);
}

.button-62:not([disabled]):hover {
 box-shadow: 0 0 .25rem rgba(0, 0, 0, 0.5), -.125rem -.125rem 1rem rgba(239, 71, 101, 0.5), .125rem .125rem 1rem rgba(255, 154, 90, 0.5);
}
</style>




-->