<template>
  <div class="tokyo_tm_portfolio">
    <div class="tokyo_tm_title">
      <div class="title_flex">
        <div class="left">
          <span>轮播图示例</span>
          <h3>SlideShow</h3>
        </div>
        <!-- End Left -->
        <div class="portfolio_filter">
          <ul>
            <li>
              <a
                v-on:click="activetab = 1"
                :class="[activetab === 1 ? 'active' : '']"
                >All</a
              >
            </li>
            <!-- End All for tabcontent 1 -->
            <!-- <li>
              <a
                v-on:click="activetab = 2"
                :class="[activetab === 2 ? 'active' : '']"
                >Vimeo</a
              >
            </li> -->
            <!-- End Vimeo tabcontent 2 -->
            <li>
              <a
                v-on:click="activetab = 3"
                :class="[activetab === 3 ? 'active' : '']"
                >Youtube</a
              >
            </li>
            <!-- End .Youtube tabcontent 3 -->
            <!-- <li>
              <a
                v-on:click="activetab = 4"
                :class="[activetab === 4 ? 'active' : '']"
                >Mix
                </a>
            </li> -->
            <!-- End Mix tabcontent 4 -->
            <li>
              <a
                v-on:click="activetab = 5"
                :class="[activetab === 5 ? 'active' : '']"
                >Gallery
                </a>
            </li>
            <!-- End Gallery tabcontent 5 -->
          </ul>
        </div>
        <!-- End .portfolio-filter -->
      </div>
    </div>
    <!-- End tokyo_tm_title -->

    <div v-if="activetab === 1" class="tabcontent">
      <ul class="portfolio_list">
        <CoolLightBox :items="allItems" :index="index" @close="index = null" :effect="'fade'">
        </CoolLightBox>
        <li
          v-for="(image, imageIndex) in allItems"
          :key="imageIndex"
          @click="index = imageIndex"
        >
          <div class="inner">
            <div class="entry tokyo_tm_portfolio_animation_wrap">
              <img class="image" :src="image.thumb" alt="Portfolio" />
            </div>
          </div>
        </li>
        <!-- End li -->
      </ul>
      <!-- End .portfolio_list -->
    </div>
    <!-- End .tabcontent 1 -->

    <div v-if="activetab === 2" class="tabcontent">
      <ul class="portfolio_list">
        <CoolLightBox :items="vimeoItems" :index="index" @close="index = null">
        </CoolLightBox>
        <li
          v-for="(image, imageIndex) in vimeoItems"
          :key="imageIndex"
          @click="index = imageIndex"
        >
          <div class="inner">
            <div class="entry tokyo_tm_portfolio_animation_wrap">
              <img class="image" :src="image.thumb" alt="Portfolio" />
            </div>
          </div>
        </li>
        <!-- End li -->
      </ul>
      <!-- End .portfolio_list -->
    </div>
    <!-- End .tabcontent 2 -->

    <div v-if="activetab === 3" class="tabcontent">
      <ul class="portfolio_list">
        <CoolLightBox
          :items="youtubeItems"
          :index="index"
          :effect="'fade'"
          @close="index = null"
        >
        </CoolLightBox>
        <li
          v-for="(image, imageIndex) in youtubeItems"
          :key="imageIndex"
          @click="index = imageIndex"
        >
          <div class="inner">
            <div class="entry tokyo_tm_portfolio_animation_wrap">
              <img class="image" :src="image.thumb" alt="Portfolio" />
            </div>
          </div>
        </li>
        <!-- End li -->
      </ul>
      <!-- End .portfolio_list -->
    </div>
    <!-- End .tabcontent 3 -->

    <div v-if="activetab === 4" class="tabcontent">
      <ul class="portfolio_list">
        <CoolLightBox :items="mixItems" :index="index" @close="index = null">
        </CoolLightBox>
        <li
          v-for="(image, imageIndex) in mixItems"
          :key="imageIndex"
          @click="index = imageIndex"
        >
          <div class="inner">
            <div class="entry tokyo_tm_portfolio_animation_wrap">
              <img class="image" :src="image.thumb" alt="Portfolio" />
            </div>
          </div>
        </li>
        <!-- End li -->
      </ul>
      <!-- End .portfolio_list -->
    </div>
    <!-- End .tabcontent 4 -->

    <div v-if="activetab === 5" class="tabcontent">
      <ul class="portfolio_list">
        <CoolLightBox
          :items="galleryItems"
          :index="index"
          :effect="'fade'"
          :useZoomBar="true"
          @close="index = null"
        >
        </CoolLightBox>

        <li
          v-for="(image, imageIndex) in galleryItems"
          :key="imageIndex"
          @click="index = imageIndex"
        >
          <div class="inner">
            <div class="entry tokyo_tm_portfolio_animation_wrap">
              <img class="image" :src="image.thumb" alt="Portfolio" />
            </div>
          </div>
        </li>
        <!-- End li -->
      </ul>
      <!-- End .portfolio_list -->
    </div>
    <!-- End .tabcontent 5 -->
  </div>
</template>

<script>
  export default {
    data() {
      return {
        activetab: 1,
        allItems: [
         {
            src: "https://youtu.be/Zv11L-ZfrSg",
            thumb: 'https://img.youtube.com/vi/Zv11L-ZfrSg/sd1.jpg',
          },
          {
            src: "https://youtu.be/WjoplqS1u18",
            thumb: 'https://img.youtube.com/vi/WjoplqS1u18/sd1.jpg',
          },
          {
            src: "https://s2.loli.net/2022/03/30/6Knboiaq1EjNft2.jpg",
            thumb: "https://s2.loli.net/2022/03/30/1W6Vor2LN4ZE98T.jpg", 
          },
          {
            src: "https://s2.loli.net/2022/03/30/TgwaUOqhy8WJQi4.jpg",
            thumb: "https://s2.loli.net/2022/03/30/ZolMiXgn7rEOu6B.jpg",
          },
        ],
        /* vimeoItems: [
          {
            src: "https://vimeo.com/246115326",
            thumb: require("../assets/img/portfolio/4.jpg"),
          },
          {
            src: "https://vimeo.com/43338103",
            thumb: require("../assets/img/portfolio/5.jpg"),
          },
        ], */
        youtubeItems: [
          {
            src: "https://youtu.be/Zv11L-ZfrSg",
            thumb: 'https://img.youtube.com/vi/Zv11L-ZfrSg/sd1.jpg',
          },
          {
            src: "https://youtu.be/WjoplqS1u18",
            thumb: 'https://img.youtube.com/vi/WjoplqS1u18/sd1.jpg',
          },
        ],
        /* mixItems: [
          {
            src: "https://vimeo.com/43338103",
            thumb: require("../assets/img/portfolio/5.jpg"),
          },
          {
            src: "https://youtu.be/ZOoVOfieAF8",
            thumb: require("../assets/img/portfolio/4.jpg"),
          },
          {
            src: require("../assets/img/portfolio/3.jpg"),
            thumb: require("../assets/img/portfolio/3.jpg"),
          },
        ], */
        galleryItems: [
          {
            src: "https://s2.loli.net/2022/03/30/wxu74ZbjlDYfOAI.jpg",
            thumb: "https://s2.loli.net/2022/03/30/bokrf2KlUBzORmc.jpg",
          },
          {
            src: "https://s2.loli.net/2022/03/30/TgwaUOqhy8WJQi4.jpg",
            thumb: "https://s2.loli.net/2022/03/30/ZolMiXgn7rEOu6B.jpg",
          },
          {
            src: "https://s2.loli.net/2022/03/30/6Knboiaq1EjNft2.jpg",
            thumb: "https://s2.loli.net/2022/03/30/1W6Vor2LN4ZE98T.jpg",
          },
          {
            src: "https://s2.loli.net/2022/03/30/4xQmgfXbtwVOFdM.jpg",
            thumb: "https://s2.loli.net/2022/03/30/YQUFH46JPIvqo2b.jpg",
          },
        ],
        index: null,
      };
    },
  };
</script>

<style lang="scss" scoped></style>
