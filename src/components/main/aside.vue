<template>
  <div id="asideMenu" class="aside">
    <ul>
      <router-link tag="li" to="/" active-class="active-link" exact>Home</router-link>
      <router-link tag="li" to="/about" active-class="active-link" exact>About</router-link>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Aside",
   methods: {
  }
};
</script>

<style scoped>
.aside {
  flex: 1;
  max-width: 250px;
  background: var(--green);
}

.aside ul {
  list-style: none;
  width: 100%;

}

.aside li {
  padding: 10px;
  margin: 15px;
  background: var(--color-transparent);
  border-radius: 3px;
  color: #f6f6f6;
  box-shadow: 0px 0px 5px #000000;
  font-weight: 600;
}

.active-link {
  background: var(--color-transparent);
  border: var(--bordered);
}

@media (max-width: 480px) {
  .aside {
    position: absolute;
    top: 0px;
    right: 0;
    max-width: 100%;
    overflow: hidden;
    width: 0%;
    height: 100%;
    background: var(--green);
    transition: all 0.5s;
    border-radius: 25px 0px 12px 0px;
  }
  
  .active-menu {
    transition: all 0.5s;
    overflow: auto;
    padding: 20px;
    width: 50%;
    height: 99%;
    box-shadow: -10px 0px 3px var(--dark);
    border: var(--bordered);
  }
  
  .aside li {
    display: flex;
    justify-content: center;
    align-items: center;
    
    box-shadow: 0px 0px 5px #000000;
    font-weight: 600;
  }
}
</style>