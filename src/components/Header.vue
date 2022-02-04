<template>
  <div class="header">
      <div class="logo">
        <img src="assets/Vue-js.png" alt="Logotipo" />
      </div>
      <div @click="activeMenu()" class="btn screen-x">
        <img src="assets/icons/menu.svg" alt="menu" />
      </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  methods: {
      activeMenu() {
        let activeMenu = document.getElementById('asideMenu')
        
        activeMenu.classList.toggle('active-menu')
      }
  }
}
</script>

<style scoped>
.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0px 20px;

    height: 60px;
    background: var(--green);
}

.logo {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  overflow: hidden;
}
.logo img{
  width: 50px;
  height: 50px;
}

  .screen-x {
    display: none;
  }

@media (max-width: 480px) {
  .screen-x {
    display: flex;
  }
}
</style>