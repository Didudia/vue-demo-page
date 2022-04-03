<template>
  <ul class="social">
    <li v-for="(social, i) in socialList" :key="i">
      <a :href="social.link" target="_blank" rel="noreferrer"
        ><img class="svg" :src="social.src" alt="social"
      /></a>
    </li>
  </ul>
  <!-- End. social -->
</template>

<script>
  export default {
    data() {
      return {
        socialList: [
         /*  {
            link: "https://www.facebook.com/",
            src: require("../assets/img/svg/social/facebook.svg"),
          }, */
          /* {
            link: "https://www.weibo.com/",
            src: require("../assets/img/svg/social/weibo.svg"),
          },
          {
            link: "https://qq.com/",
            src: require("../assets/img/svg/social/qq.svg"),
          },
          {
            link: "https://www.douyin.com/",
            src: require("../assets/img/svg/social/tik-tok.svg"),
          },
          {
            link: "https://www.wechat.com/",
            src: require("../assets/img/svg/social/wechat.svg"),
          },*/
          {
            link: "https://github.com/Didudia",
            src: require("../assets/img/svg/social/github.svg"),
          },
        ],
      };
    },
  };
</script>

<style lang="scss" scoped></style>
