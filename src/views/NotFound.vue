<template>
  <div class="not-found-wrapper">
    <div class="leftpart">
      <div class="leftpart_inner">
        <div class="logo">
          <router-link to="/"
            ><img src="../assets/img/logo/1.png" alt="brand"
          /></router-link>
        </div>
        <div class="copyright">
          <p>
            &copy; {{ new Date().getFullYear() }} Website <br />
            Created by<a
              href="https://didudia.github.io/"
              target="_blank"
              rel="noreferrer"
              >MichaelWang</a
            >
          </p>
        </div>
      </div>
    </div>
    <!-- End .leftpart -->
    <div class="rightpart">
      <div class="rightpart_in">
        <div class="tokyo_tm_section">
          <div class="container">
            <div class="tokyo_tm_error">
              <div class="tokyo_tm_error_inner">
                <h1>404!</h1>
                <h3>Page not found</h3>
                <p>The page you were looking for could not be found.</p>
                <router-link class="ib-button" to="/">Go to Home</router-link>
              </div>
            </div>
            <!-- End .tokyo_tm_error -->
          </div>
        </div>
      </div>
    </div>
    <!-- End .rightpart -->
    <footer class="footer-wrapper">
      <div class="copyright">
        <p>
          © 2022 Website Created by<a
            href="https://didudia.github.io/"
            target="_blank"
            rel="noreferrer"
            >MichaelWang</a
          >
        </p>
      </div>
    </footer>
    <!-- End .footer-wrapper -->
  </div>
</template>
