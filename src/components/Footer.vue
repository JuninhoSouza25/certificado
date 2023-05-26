<template>
  <footer>
    <img src="../assets/logotipo-1-principal.svg" alt="logo Academy Abroad"/>
    <div class="assinatura-container">
        <div></div>
        <h3>Dr. Rafael Kenji</h3>
        <p>CEO</p>
    </div>

  </footer>
</template>

<script>

export default {
  name: "FooterComponent"
}

</script>

<style>

footer {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

footer img {
  width: 200px;
  margin-left: 40px;
}

.assinatura-container {
  text-align: center;
}

.assinatura-container div {
  width: 170px;
  height: 2px;
  background-color: black;
}

</style>