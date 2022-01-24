<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="info">
        <b-navbar-brand href="/">This Example Blog</b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>

        </b-navbar-nav>

        <b-navbar-nav class="ml-auto">
          <b-nav-item v-for="item in menu" :key="item.id" :to="item.link">{{ item.name }}</b-nav-item>
        </b-navbar-nav>
        </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  props: {
    menu: {
      type: Array,
      default: Array
    }
  }
}
</script>
