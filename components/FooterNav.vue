<template>
  <footer class="footer footer-nav">
    <div class="container">
      <div class="columns">
        <div class="column is-3">
          <div class="footer-link-title site-name">
            <n-link to="/">
              Design Influences
            </n-link>
          </div>
        </div>
        <div class="column is-3 menu-imagine">
          <h3 class="footer-link-title">
            <n-link to="/imagine">
              Imagine
            </n-link>
          </h3>
          <div class="footer-links">
            <div class="footer-link">
              <n-link to="/imagine/resources">
                Resources
              </n-link>
            </div>
            <div class="footer-link">
              <n-link to="/imagine/theory">
                Theory
              </n-link>
            </div>
            <div class="footer-link">
              <n-link to="/imagine/research">
                Research
              </n-link>
            </div>
            <div class="footer-link">
              <n-link to="/imagine/strategy">
                Strategy
              </n-link>
            </div>
          </div>
        </div>
        <div class="column is-3 menu-design">
          <h3 class="footer-link-title">
            <n-link to="/design">
              Design
            </n-link>
          </h3>
          <div class="footer-links">
            <div class="footer-link">
              <n-link to="/design/ethics">
                Ethics
              </n-link>
            </div>
            <div class="footer-link">
              <n-link to="/design/principles">
                Principles
              </n-link>
            </div>
            <div class="footer-link">
              <n-link to="/design/processes">
                Processes
              </n-link>
            </div>
            <div class="footer-link">
              <n-link to="/design/systems">
                Systems
              </n-link>
            </div>
          </div>
        </div>
        <div class="column is-3 menu-build">
          <h3 class="footer-link-title">
            <n-link to="/build">
              Build
            </n-link>
          </h3>
          <div class="footer-links">
            <div class="footer-link">
              <n-link to="/build/people">
                People
              </n-link>
            </div>
            <div class="footer-link">
              <n-link to="/build/relationships">
                Relationships
              </n-link>
            </div>
            <div class="footer-link">
              <n-link to="/build/community">
                Community
              </n-link>
            </div>
            <div class="footer-link">
              <n-link to="/build/social-architecture">
                Social Architecture
              </n-link>
            </div>
          </div>
        </div>
      </div>
      <div class="siteinfo">
        <div class="social-media">
          <a class="medium" href="https://medium.com/builderscollective">
            <b-icon icon="medium" />
          </a>
          <a class="twitter" href="https://twitter.com/bldrsco">
            <b-icon icon="twitter-box" />
          </a>
          <a class="facebook" href="https://www.facebook.com/bldrscollective">
            <b-icon icon="facebook-box" />
          </a>
          <a class="instagram" href="https://www.instagram.com/bldrsco">
            <b-icon icon="instagram" />
          </a>
        </div>
        <p class="credit">
          A project of the&nbsp;
          <a href="https://builderscollective.com">
            builders collective
          </a>
        </p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterNav'
}
</script>

<style lang="scss">
@import '../assets/css/variables.scss';

.footer-nav {
  background: #333;
  color: #fff;
  a {
    color: #999;
    &:hover {
      color: #00aeef;
    }
  }
  .menu-design {
    a:hover {
      color: $secondary;
    }
  }
  .menu-build {
    a:hover {
      color: $tertiary;
    }
  }
}

.footer-link-title {
  font-size: 1.3rem;
  margin-bottom: 1rem;
  a {
    color: #fff;
    display: block;
  }
}

.footer-link {
  a {
    display: block;
    padding-top: 0.25em;
    padding-bottom: 0.25em;
  }
}

.siteinfo {
  font-size: 0.9rem;
  color: #666;
  border-top: 1px solid #444;
  margin-top: 3rem;
  padding-top: 2rem;
  .social-media {
    margin-bottom: 1rem;
    a {
      margin-right: 1rem;
      color: #666;
      .icon {
        height: 30px;
        width: 30px;
        font-size: 30px;
        .mdi:before {
          font-size: 30px;
        }
      }
      &:hover {
        color: #00aeef;
      }
    }
  }
}

@media screen and (min-width: 768px) {
  .siteinfo {
    .social-media {
      float: right;
      a {
        margin-left: 1rem;
        margin-right: 0;
      }
    }
    p.credit {
      margin-top: 0.3rem;
    }
  }
}
</style>
