<template>
  <div class="footer">
    <a href="https://github.com/theluposki" target="_blank">@theluposki</a>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
.footer {
  display: flex;
  align-items: center;
  padding: 0px 20px;
  height: 30px;
  background: var(--green);
}

.footer a {
  text-decoration: none;
  font-size: 14px;
  font-weight: 600;
  color: var(--white);
}
</style>