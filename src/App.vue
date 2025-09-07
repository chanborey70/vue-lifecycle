<template>
<HeroArea v-if="!remove"></HeroArea>
<button @click="changeValue">Remove from DOM</button>
<ServiceSection></ServiceSection>
<AboutSection></AboutSection>
<WhySection></WhySection>
<TeamSection></TeamSection>
<ClientSection></ClientSection>
<InfoSection></InfoSection>
<FooterSection></FooterSection>
</template>

<script>
import HeroArea from './components/HeroArea.vue';
import ServiceSection from './components/ServiceSection.vue';
import AboutSection from './components/AboutSection.vue';
import WhySection from './components/WhySection.vue';
import TeamSection from './components/TeamSection.vue';
import ClientSection from './components/ClientSection.vue';
import InfoSection from './components/InfoSection.vue';
import FooterSection from './components/FooterSection.vue';
export default {
  data() {
    return {
      remove: false,
    };
  },
  methods: {
    changeValue() {
      this.remove = !this.remove;
    },
  },

// Regigstere component
  components: {
    HeroArea,
    ServiceSection,
    AboutSection,
    WhySection,
    TeamSection,
    ClientSection,
    InfoSection,
    FooterSection,
  }
}
</script>
