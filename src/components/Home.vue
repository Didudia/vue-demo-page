<template>
  <div class="tokyo_tm_home">
    <div class="home_content">
      <div class="avatar">
        <div
          class="image avatar_img"
          :style="{ backgroundImage: 'url(' + src1 + ')' }"
        ></div>
      </div>
      <!-- End .avatar -->
      <div class="details">
        <h3 class="name">Michael Wang</h3>
        <p class="job">
          人生得意须尽欢，莫使金樽空对月
        </p>

        <Social />
      </div>
      <!-- End .details -->
    </div>
  </div>
</template>

<script>
  import Social from "./Social";
  export default {
    components: {
      Social,
    },
    data() {
      return {
        src1: "https://s2.loli.net/2022/04/07/NXoUDl6H9Eia2JQ.jpg",
      };
    },
  };
</script>

<style lang="scss"></style>
