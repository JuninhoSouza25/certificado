<template>
  <section>
    <div>
      <h2>{{ jsonData.nome }}</h2>
      <p>concluiu o curso online com carga horária de {{ jsonData.duracao }} horas.</p>
      <p id="finalizacao">Finalizado na data de {{ jsonData.data }}.</p>
    </div>
    <div>
      <p>Curso</p>
      <h2>{{ textoMaiusculo }}</h2>
    </div>
  </section>
</template>

<script>

export default {
  name: "SectionComponent",
  data() {
    return {
      jsonData: [],
    };
  },
  mounted() {
    this.fetchData();
  },
  methods: {
    fetchData() {
      this.jsonData = require('../api/data.json');
    }
  },
  computed: {
    textoMaiusculo(){
      const curso = this.jsonData.curso || '';
      return curso
    }
  }
  
}

</script>

<style scoped>

section {
  width: 90%;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  gap: 50px;
}

h2 {
  font-size: 56px;
}

p {
  font-size: 28px;
}

#finalizacao {
  font-size: 22px;
  font-weight: 200;
}

</style>