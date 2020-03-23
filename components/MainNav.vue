<template>
  <nav
    class="navbar header is-fixed-top"
    role="navigation"
    aria-label="main navigation"
  >
    <div class="container">
      <div class="navbar-brand">
        <n-link class="navbar-item" to="/">
          <strong>
            Design Influences
          </strong>
        </n-link>
        <div
          class="navbar-burger"
          :class="{ 'is-active': showNav }"
          @click="showNav = !showNav"
        >
          <span aria-hidden="true" />
          <span aria-hidden="true" />
          <span aria-hidden="true" />
        </div>
      </div>
      <div id="main-menu" class="navbar-menu" :class="{ 'is-active': showNav }">
        <div class="navbar-start">
          <div class="navbar-item has-dropdown is-hoverable menu-imagine">
            <n-link class="navbar-link" to="/imagine">
              Imagine
            </n-link>
            <div class="navbar-dropdown">
              <n-link class="navbar-item" to="/imagine/resources">
                Resources
              </n-link>
              <n-link class="navbar-item" to="/imagine/theory">
                Theory
              </n-link>
              <n-link class="navbar-item" to="/imagine/research">
                Research
              </n-link>
              <n-link class="navbar-item" to="/imagine/strategy">
                Strategy
              </n-link>
            </div>
          </div>
          <div class="navbar-item has-dropdown is-hoverable menu-design">
            <n-link class="navbar-link" to="/design">
              Design
            </n-link>
            <div class="navbar-dropdown">
              <n-link class="navbar-item" to="/design/ethics">
                Ethics
              </n-link>
              <n-link class="navbar-item" to="/design/principles">
                Principles
              </n-link>
              <n-link class="navbar-item" to="/design/processes">
                Processes
              </n-link>
              <n-link class="navbar-item" to="/design/systems">
                Systems
              </n-link>
            </div>
          </div>
          <div class="navbar-item has-dropdown is-hoverable menu-build">
            <n-link class="navbar-link" to="/build">
              Build
            </n-link>
            <div class="navbar-dropdown">
              <n-link class="navbar-item" to="/build/people">
                People
              </n-link>
              <n-link class="navbar-item" to="/build/relationships">
                Relationships
              </n-link>
              <n-link class="navbar-item" to="/build/community">
                Community
              </n-link>
              <n-link class="navbar-item" to="/build/social-architecture">
                Social Architecture
              </n-link>
            </div>
          </div>
        </div>
        <div class="navbar-end">
          <n-link class="navbar-item menu-about" to="/about">
            About
          </n-link>
          <n-link class="navbar-item menu-journal" to="/journal">
            Journal
          </n-link>
          <n-link class="navbar-item menu-work" to="/work">
            Work
          </n-link>
          <n-link class="navbar-item menu-resources" to="/resources">
            Resources
          </n-link>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'MainNav',
  data() {
    return {
      showNav: false
    }
  }
}
</script>

<style lang="scss">
@import '../assets/css/variables.scss';
#main-menu {
  .menu-imagine {
    &.navbar-item.has-dropdown:hover {
      .navbar-link {
        background-color: $primary;
        color: #fff;
        &:not(.is-arrowless)::after {
          border-color: #fff;
        }
      }
    }
    .navbar-link {
      &:hover {
        color: #fff;
      }
      &:not(.is-arrowless)::after {
        border-color: $primary;
      }
    }
  }

  .menu-design {
    &.navbar-item.has-dropdown:hover {
      .navbar-link {
        background-color: $secondary;
        color: #fff;
        &:not(.is-arrowless)::after {
          border-color: #fff;
        }
      }
    }
    .navbar-link {
      &:hover {
        color: #fff;
      }
      &:not(.is-arrowless)::after {
        border-color: $secondary;
      }
    }
  }

  .menu-build {
    &.navbar-item.has-dropdown:hover {
      .navbar-link {
        background-color: $tertiary;
        color: #fff;
        &:not(.is-arrowless)::after {
          border-color: #fff;
        }
      }
    }
    .navbar-link {
      &:hover {
        color: #fff;
      }
      &:not(.is-arrowless)::after {
        border-color: $tertiary;
      }
    }
  }

  @media screen and (min-width: 1024px) {
    .menu-imagine {
      .navbar-dropdown {
        a.navbar-item {
          &:hover {
            background-color: $primary;
            color: #fff;
          }
        }
      }
    }
    .menu-design {
      .navbar-dropdown {
        a.navbar-item {
          &:hover {
            background-color: $secondary;
            color: #fff;
          }
        }
      }
    }
    .menu-build {
      .navbar-dropdown {
        a.navbar-item {
          &:hover {
            background-color: $tertiary;
            color: #fff;
          }
        }
      }
    }
  }

  .navbar-item.is-hoverable:focus .navbar-dropdown,
  .navbar-item.is-hoverable:focus-within .navbar-dropdown {
    display: none;
  }
  .navbar-item.is-hoverable:hover .navbar-dropdown {
    display: block;
  }

  .menu-design .nuxt-link-active {
    color: $secondary;
  }
  .menu-build .nuxt-link-active {
    color: $tertiary;
  }
  a.navbar-link:focus-within,
  a.navbar-item:hover,
  a.navbar-item:focus,
  a.navbar-item.nuxt-link-active {
    background-color: transparent;
  }
}
</style>
