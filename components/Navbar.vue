<template>
  <div>
    <b-navbar toggleable="lg" type="dark" class="navbar">
      <b-navbar-brand href="/" class="ml-6">
        홈
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse" />

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="mx-auto">
          <b-nav-item href="/request">
            과제물
          </b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>
<style scoped>
.navbar {
    background-color: #3fb984;
}
</style>
