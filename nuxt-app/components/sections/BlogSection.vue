<template>
  <b-container>
    <b-row>
      <b-col v-for="post in posts" :key="post.id" lg="6">
        <Card :post="post" />
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import Card from '../Card.vue'

export default {
  name: 'BlogSection',
  components: {
    Card,
  },
  props: {
    posts: {
      type: Array,
      default: Array,
    }
  }
}
</script>