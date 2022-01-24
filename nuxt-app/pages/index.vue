<template>
  <div>
    <NavbarSection :menu="menu"/>
    <BlogSection :posts="posts" />
    <FooterSection />
  </div>
</template>

<script>
import NavbarSection from '@/components/sections/NavbarSection.vue'
import BlogSection from '@/components/sections/BlogSection.vue'
import FooterSection from '@/components/sections/FooterSection.vue'

export default {
  name: 'IndexPage',
  components: {
    NavbarSection,
    BlogSection,
    FooterSection,
  },
  data() {
    return {
      menu: [
        { "id": 1, "name": "Home", "link": "/" },
        { "id": 2, "name": "Blog", "link": "b" },
        { "id": 3, "name": "About", "link": "about" },
      ],
      posts: [
        {"id": 1, "title": "Horizontal Card 1", "desc": "This is a wider card with" },
        {"id": 2, "title": "Horizontal Card 2", "desc": "This is a wider card with" },
        {"id": 3, "title": "Horizontal Card 3", "desc": "This is a wider card with" },
        {"id": 4, "title": "Horizontal Card 4", "desc": "This is a wider card with" },
        {"id": 5, "title": "Horizontal Card 5", "desc": "This is a wider card with" },
        {"id": 6, "title": "Horizontal Card 6", "desc": "This is a wider card with" },
      ]
    }
  },
}
</script>
