<template>
  <div class="main">
      <Section />
      <Aside />
  </div>
</template>

<script>
import Section from "../components/main/section.vue";
import Aside from "../components/main/aside.vue";

export default {
  name: 'Main',
    components: {
      Section,
      Aside
  }
}
</script>

<style scoped>
.main {
    position: relative;
    flex: 1;
    overflow: hidden;
    display: flex;
    gap: 3px;
}
</style>