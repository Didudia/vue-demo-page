<template>
  <div class="tokyo_tm_intro">
    <!-- <div class="tokyo_tm_intro_fixed_price">
      <span class="anim"></span><span class="anim"></span
      ><span class="anim"></span
      ><a
        href="https://themeforest.net/item/tokyo-vuejs-personal-portfolio-template/32797372"
        target="_blank"
        class="pricing-info anim"
        >-78%</a
      >
    </div> -->
    <!-- End .tokyo_tm_intro_fixed_price -->

    <div class="short_info">
      <router-link to="/">
        <img src="../assets/img/logo/1.png" alt="brand" />
      </router-link>

      <h3>基于VUE的个人页展示</h3>
    </div>
    <!-- End .short_info -->

    <!-- <span class="intro_line"></span> -->
    <span class="intro_line_2"></span>
    <!-- <span class="intro_line_3"></span> -->

    <div class="demos">
      <div class="left">
        <router-link to="/home-light" target="_blank">
          <div class="desc">
            <img src="https://s2.loli.net/2022/04/07/9PZBwiaR8eUtKNx.png" alt="light version demo" />
            <h3 class="title">Light Demo</h3>
          </div>
        </router-link>
      </div>
      <!-- End .left -->
      <div class="right">
        <router-link to="/home-dark" target="_blank"
          ><div class="desc">
            <img src="https://s2.loli.net/2022/04/07/rHvwxFSULeN6ig8.png" alt="dark version demo" />
            <h3 class="title">Dark Demo</h3>
          </div></router-link
        >
      </div>
      <!-- End .right -->
    </div>
    <!-- End .demos -->
  </div>
  <!-- End .tokyo_tm_intro -->
</template>

<script>
export default {};
</script>

<style lang="scss" scoped></style>
