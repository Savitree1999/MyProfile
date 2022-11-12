<template>
  <div>
    <NavigationVue />
    <HeadVue />
    <ContentVue />
    <FooterVue />
  </div>
</template>

<script>
import HeadVue from "@/components/layout/HeadVue.vue";
import ContentVue from "@/components/layout/ContentVue.vue";
import FooterVue from "@/components/layout/FooterVue.vue";
import NavigationVue from "@/components/layout/NavigationVue.vue";


export default {
  components: {
    HeadVue,
    ContentVue,
    FooterVue,
    NavigationVue,
    
  },
};
</script>

<style>
</style>
