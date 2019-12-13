<template>
  <section>
    <Header />
    <AboutSection />
    <FeaturesSection />
    <ToursSection />
  </section>
</template>

<script>
import Header from '~/components/Header.vue'
import AboutSection from '~/components/AboutSection.vue'
import FeaturesSection from '~/components/FeaturesSection.vue'
import ToursSection from '~/components/ToursSection.vue'

export default {
  components: {
    Header,
    AboutSection,
    FeaturesSection,
    ToursSection
  }
}
</script>

<style scoped lang="scss"></style>
