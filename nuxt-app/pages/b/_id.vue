<template>
  <div>
    <NavbarSection :menu="menu"/>
    <p> This _id</p>
    <FooterSection />
  </div>
</template>

<script>
import NavbarSection from '@/components/sections/NavbarSection.vue'
import FooterSection from '@/components/sections/FooterSection.vue'

export default {
  name: 'PostPage',
  components: {
    NavbarSection,
    FooterSection,

  },
  data() {
    return {
      menu: [
        { "id": 1, "name": "Home", "link": "/" },
        { "id": 2, "name": "Blog", "link": "b" },
        { "id": 3, "name": "About", "link": "about" },
      ],
    }
  },
}
</script>