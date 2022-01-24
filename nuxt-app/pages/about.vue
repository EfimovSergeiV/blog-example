<template>
  <div class="about">
    <NavbarSection :menu="menu"/>
    <MITSection />
    <FooterSection />
  </div>
</template>

<script>
import NavbarSection from '@/components/sections/NavbarSection.vue'
import FooterSection from '@/components/sections/FooterSection.vue'
import MITSection from '@/components/sections/MITSection.vue'

export default {
  name: 'AboutPage',
  components: {
    NavbarSection,
    FooterSection,
    MITSection,
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
