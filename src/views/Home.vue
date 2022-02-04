<template>
  <div class="home">
        <h1 class="text-h">Vue Js 😽</h1>
        <p class="text-p">Vue (pronunciado /vjuː/, como view ) é um framework progressivo para construir interfaces de usuário. Ao contrário de outros frameworks monolíticos, o Vue é projetado desde o início para ser adotável de forma incremental. A biblioteca principal está focada apenas na camada de visualização e é fácil de pegar e integrar com outras bibliotecas ou projetos existentes. Por outro lado, o Vue também é perfeitamente capaz de alimentar aplicativos sofisticados de página única quando usado em combinação com ferramentas modernas e bibliotecas de suporte .</p>
        <div class="link-c">
          <a href="https://vuejs.org/v2/guide/" target="_blank">vuejs.org</a>
        </div>
        
        <div class="img-c">
          <img src="assets/vue-code01.jpg" alt="code 01" />
        </div>
        <div class="img-c">
          <img src="assets/vue-code02.jpg" alt="code 02" />
        </div>
  </div>
</template>

<script>
export default {
  name: 'Home',
}
</script>

<style scoped>
.home {
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    overflow: scroll;
}

.text-h {
  width: 100%;
  font-size: 33px;
  padding: 20px;
  text-align: center;
  color: var(--green);
  text-shadow: 2px 0px 3px var(--dark);
}

.text-p {
  line-height: 2em;
  font-weight: 400;
  color: #777777;
}

.link-c {
  width: 100%;
  padding: 20px;
  text-align: right;
}
.link-c a {
  text-decoration: none;
  font-weight: 800;
  color: var(--green);
}

.img-c {
  width: 300px;
  height: 300px;
  min-width: 300px;
  min-height: 300px;
  margin: 20px 0px;
  display: flex;
  justify-content: center;
  align-items: center;
  box-shadow: 0px 0px 12px var(--dark);
}
.img-c img {
  width: 300px;
  height: 300px;
}

</style>