<template>
  <div class="tokyo_tm_about">
    <div class="about_image">
      <img src="https://s2.loli.net/2022/04/07/NXoUDl6H9Eia2JQ.jpg" alt="about" />
    </div>
    <!-- End .about_image -->

    <div class="description">
      <h3 class="name">Michael Wang &amp; 前端开发工程师</h3>
      <div class="description_inner">
        <div class="left">
          <p>
            基于Vue搭建的响应式个人展示页<br>
            轮播图由vue-cool-lightbox插件提供<br>博客页面展示，符合seo基本规则<br>
            示例图片由<a href="https://sm.ms/">sm.ms图床</a>提供存储，<a href="https://www.cloudflare.com/" target="_blank">CloudFlare</a>提供CDN<br>
            项目地址托管在<a href="https://github.com/Didudia/vue-demo-page" target="_blank">Github</a>，
            部署在<a href="https://vercel.com/" target="_blank">vercel</a>
          </p>
          <!-- <div class="tokyo_tm_button">
            <button class="ib-button" @click="showModal">Read More</button>
          </div> -->
        </div>
        <!-- End .left -->

        <div class="right">
          <ul>
            <!-- <li>
              <p><span>Birthday:</span>1998</p>
            </li> -->
            <li>
              <p><span>年龄:</span>24</p>
            </li>
            <!-- <li>
              <p><span>住址:</span>东莞东城</p>
            </li> -->
            <li>
              <p>
                <span>邮箱:</span
                ><a href="mailto:1064878181@qq.com">1064878181@qq.com</a>
              </p>
            </li>
            <!-- <li>
              <p>
                <span>联系电话:</span
                >+86 17802031811
              </p>
            </li> -->
            <li>
              <p><span>个人网站:</span><a href="https://didudia.github.io/" target="_blank">https://didudia.github.io</a></p>
            </li>
            <li>
              <p><span>Github:</span><a href="https://github.com/Didudia" target="_blank">https://github.com/Didudia</a></p>
            </li>
          </ul>
          <!-- End ul -->
        </div>
        <!-- End .right -->
      </div>
    </div>

    <!-- Start Modalbox -->
    <transition name="fade">
      <!-- Modal -->
      <div
        :class="{ 'modal-mask': isActive }"
        id="modal"
        @click="closeModal"
        v-if="isVisible"
      >
        <div
          class="modal-dialog modal-dialog-centered modal-dialog-scrollable modal-user"
          @click.stop
        >
          <div class="modal-content">
            <div class="tokyo_tm_modalbox_about">
              <div class="close" @click="closeModal">
                <img
                  class="svg"
                  src="../assets/img/svg/cancel.svg"
                  alt="cancel-img"
                />
              </div>
              <!-- End .close -->
              <div class="my_box">
                <div class="left">
                  <div class="about_title">
                    <h3>Job Skills</h3>
                  </div>
                  <!-- End .abut_title -->
                  <div class="tokyo_progress">
                    <div class="progress_inner">
                      <span
                        ><span class="label">Wedding Photography</span
                        ><span class="number">95%</span></span
                      >
                      <div class="background">
                        <div class="bar">
                          <div class="bar_in" style="width:95%"></div>
                        </div>
                      </div>
                    </div>
                    <!-- End progress_inner -->
                    <div class="progress_inner">
                      <span
                        ><span class="label">Lifestyle Photography</span
                        ><span class="number">80%</span></span
                      >
                      <div class="background">
                        <div class="bar">
                          <div class="bar_in" style="width:80%"></div>
                        </div>
                      </div>
                    </div>
                    <!-- End progress_inner -->
                    <div class="progress_inner">
                      <span
                        ><span class="label">Family Photography</span
                        ><span class="number">90%</span></span
                      >
                      <div class="background">
                        <div class="bar">
                          <div class="bar_in" style="width:90%"></div>
                        </div>
                      </div>
                    </div>
                    <!-- End progress_inner -->
                  </div>
                  <!-- End .tokyo_progress -->
                </div>
                <!-- End .left -->
                <div class="right">
                  <div class="about_title">
                    <h3>Language Skills</h3>
                  </div>
                  <div class="tokyo_progress">
                    <div class="progress_inner">
                      <span
                        ><span class="label">English</span
                        ><span class="number">95%</span></span
                      >
                      <div class="background">
                        <div class="bar">
                          <div class="bar_in" style="width:95%"></div>
                        </div>
                      </div>
                    </div>
<!--                     <div class="progress_inner">
                      <span
                        ><span class="label">Japanese</span
                        ><span class="number">90%</span></span
                      >
                      <div class="background">
                        <div class="bar">
                          <div class="bar_in" style="width:90%"></div>
                        </div>
                      </div>
                    </div>
                    <div class="progress_inner">
                      <span
                        ><span class="label">Arabian</span
                        ><span class="number">85%</span></span
                      >
                      <div class="background">
                        <div class="bar">
                          <div class="bar_in" style="width:85%"></div>
                        </div>
                      </div>
                    </div> -->
                  </div>
                </div>
                <!-- End .right -->
              </div>
              <!-- <div class="counter">
                <div class="about_title">
                  <h3>Fun Facts</h3>
                </div>
                <ul>
                  <li>
                    <div class="list_inner">
                      <h3>777+</h3>
                      <span>Projects Completed</span>
                    </div>
                  </li>
                  <li>
                    <div class="list_inner">
                      <h3>3K</h3>
                      <span>Happy Clients</span>
                    </div>
                  </li>
                  <li>
                    <div class="list_inner">
                      <h3>9K+</h3>
                      <span>Lines of Code</span>
                    </div>
                  </li>
                </ul>                
              </div> -->
              <!-- End .counter -->
              <div class="partners">
                <div class="about_title">
                  <h3>hooper轮播组件</h3>
                </div>
                <Brand />
              </div>
              <!-- End .partner -->
            </div>
            <!-- End .tokyo_tm_modalbox_about -->
          </div>
        </div>
      </div>
    </transition>
    <!-- End Modalbox -->
  </div>
</template>

<script>
import Brand from "./Brand";
export default {
  components: {
    Brand,
  },
  data() {
    return {
      isActive: false,
      isVisible: false,
    };
  },
  methods: {
    showModal: function() {
      this.isActive = true;
      this.isVisible = true;
    },
    closeModal: function() {
      this.isActive = false;
      this.isVisible = false;
    },
  },
};
</script>

<style lang="scss"></style>
