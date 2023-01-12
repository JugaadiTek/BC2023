<script setup>
defineProps({
  formcontent: []
})
</script>
<template>
  <section id="getintouch" class="" role="banner">
    <div class="container">
      <div class="inner-container">
        <div class="content-block ">
          <h2>Get In Touch</h2>
          <p>We can help you put the pieces together for a optimized and fully implemented GTM Strategy</p>
          <!-- <form action="">
            <label for="fname">First name</label>
            <input type="text" id="fname" name="fname">

            <label for="lname">Last name</label>
            <input type="text" id="lname" name="lname">

            <label for="workemail">Work Email</label>
            <input type="text" id="workemail" name="workemail">

            <label for="title">title</label>
            <input type="text" id="title" name="title">

            <input type="submit" value="send">
          </form> -->

          <form action="">
            <div>
              <label for="fname">First name</label>
              <input type="text" id="fname" name="fname">
            </div>

            <div><label for="lname">Last name</label>
              <input type="text" id="lname" name="lname">
            </div>

            <div>
              <label for="workemail">Work Email</label>
              <input type="text" id="workemail" name="workemail">
            </div>

            <div>
              <label for="title">title</label>
              <input type="text" id="title" name="title">
            </div>

            <div>
              <input type="submit" value="send">
            </div>

          </form>

        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.container {
  background-color: black;
  color: white;
  text-align: left;
}

div.content-block {
  padding: 50px;
}

div.content-block>h2 {
  padding: 10px 10px 0 10px;
  margin: 2px;
  font-size: 32px;
}

div.content-block>p {
  padding: 0 10px 10px 10px;
  margin: 2px;
  font-size: 20px;
}

form>div {
  display: inline-block;
  padding: 10px;
}

form>div>input {
  display: block;
  padding: 5px;
  margin-top: 10px;
}

form>div>input:last-child {
  /* couldn't style button, it needs to be same as input forms and responsive */
}
</style>
