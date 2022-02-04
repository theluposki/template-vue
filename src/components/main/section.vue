<template>
  <div class="section">
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: "Section",
};
</script>

<style scoped>
.section {
  flex: 1;
  display: flex;
  overflow: hidden;
  padding: 10px 20px;
  background: var(--white);
}
</style>