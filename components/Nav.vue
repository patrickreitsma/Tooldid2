<template>
  <nav class="nav">
    <nav class="mobile">
      <b-navbar toggleable type="dark" variant="dark">
        <b-navbar-toggle target="nav_text_collapse" />
        <b-collapse is-nav id="nav_text_collapse">
          <b-navbar-nav>
            <b-nav-text><nuxt-link to="/">Home</nuxt-link></b-nav-text>
            <b-nav-text><nuxt-link to="Games">Games</nuxt-link></b-nav-text>
            <b-nav-text><nuxt-link to="Series">Series</nuxt-link></b-nav-text>
            <b-nav-text><nuxt-link to="Movies">Movies</nuxt-link></b-nav-text>
            <b-nav-text><nuxt-link to="Contact">Contact</nuxt-link></b-nav-text>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </nav>
    <div class="desktop">
      <ul class="desktopul">
        <li><nuxt-link to="/">Home</nuxt-link></li>
        <li><nuxt-link to="Games">Games</nuxt-link></li>
        <li><nuxt-link to="Series">Series</nuxt-link></li>
        <li><nuxt-link to="Movies">Movies</nuxt-link></li>
        <li><nuxt-link to="Contact">Contact</nuxt-link></li>
      </ul>
    </div>
  </nav>
</template>

<script>
</script>

<style scoped lang="scss">
  .desktop {
    display: none;
  }
  .mobile {
    width: 100%;
  }
  .navbar {
    width: 100%;
    background-color: #0d1319 !important;
  }
  .navbar-toggler {
    width: 100%;
    border-color: white;
  }
  .navbar-nav {
    align-items: center;
  }
  .navbar-text {
    color: #ffffff;
  }
  @include breakpoint(l) {
    .desktop {
      background: #0d1319;
      width: 100%;
      height: 56px;
      display: flex;
      justify-content: flex-end;
      align-items: center;
    }
    ul {
      width: 100%;
      display: flex;
      justify-content: flex-end;
      padding-right: 5px;
    }
    ul li {
      display: inline-block;
      color: #ffffff;
    }
    li {
      width: 10%;
    }
    .mobile {
      display: none;
    }
  }
</style>
