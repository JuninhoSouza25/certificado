<template>
  <nav>
    <h1>
      <text style="font-weight: 700; font-size: 84px;">CERTIFICADO</text><br> DE CONCLUSÃO
    </h1>
    <div id="element"></div>
  </nav>
</template>

<script>

export default {
  name: "NavComponent",
}

</script>

<style scoped>
nav {
  width: 90%;
  display: flex;
  align-items: flex-end;
}

h1 {
  font-size: 56px;
  font-weight: 100;
  color: var(--preto);
}

#element {
  width: 20px;
  height: 20px;
  border-radius: 50%;
  background-color: var(--azul);
  margin-left: -150px;
  margin-bottom: 10px;
}
</style>