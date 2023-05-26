<template>
  <div class="frame">
    <div class="area-1">
      <NavComponent />
      <SectionComponent />
      <FooterComponent />
    </div>
    <div class="area-2">
      <img class="logo-mini" src="./assets/logotipo-4-azul.svg" alt="logo Academy Abroad"/>
    </div>
  </div>
</template>

<script>
import NavComponent from './components/Nav.vue'
import SectionComponent from './components/Content.vue'
import FooterComponent from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    NavComponent,
    SectionComponent,
    FooterComponent
  }
}
</script>

<style>
:root {
  --azul: #1780ff;
  --preto: #2A2B2E;
  --creme: #F3F8F2;
  --font: 'Ubuntu', sans-serif;
}

#app, *, html {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: var(--font);
  color: var(--preto);
}

.frame {
  margin: 20px;
  background-color: var(--creme);
  background-image: url('./assets/logotipo-reduzido-5-positivo.svg');
  background-repeat: no-repeat;
  width: 1500px;
  height: 900px;
  border-radius: 15px;
  display: flex;
  justify-content: start;
}

.area-1 {
  width: 90%;
  height: 100%;
  display: flex;
  justify-content: space-around;
  align-items: flex-end;
  flex-direction: column;
}

.logo-mini {
  transform: rotate(-90deg);
  width: 100%;
}

.area-2 {
  background: var(--azul);
  background-image: url('./assets/logotipo-reduzido-4-azul.svg');
  width: 10%;
  height: 100%;
  border-radius: 0 15px 15px 0;
  display: flex;
  align-items: flex-end;
  justify-content: flex-end;
  padding-bottom: 70px;
}

</style>
