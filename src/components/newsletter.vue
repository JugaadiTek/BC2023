<script setup>
</script>

<template>
      <div class="inner-container">
        <div class="content-block ">
          <form action="">
            <!-- check if this is right way to do  -->
            <span>
              <h2>Join Our Newsletter</h2>
            </span>

            <span>
              <label for="fname">First name</label>
              <input type="text" id="fname" name="fname" placeholder="First Name">
            </span>

            <span>
              <label for="lname">Last name</label>
              <input type="text" id="lname" name="lname" placeholder="Last Name">
            </span>

            <span>
              <label for="workemail">Email</label>
              <input type="text" id="workemail" name="workemail" placeholder="Email">
            </span>

            <span><input type="submit" value="Sign Up"></span>

          </form>
        </div>
      </div>
</template>

<style scoped >

form>span {
  display: inline-block;
  text-align: left;
  padding: 10px;

}

form>span>input {
  display: block;
  padding: 5px;
  margin-top: 10px;
}

form > span:last-child > input {
  border: 2px solid var() ;
}

label {
  color: var(--primary);
}
</style>