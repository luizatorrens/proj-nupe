<script>
export default {
  props: ["categoria"],
};
</script>

<template>
  <h1 :class="categoria.cor">{{ categoria.nome }}</h1>

  <div class="card-group">
    <div
      class="card card-material"
      v-for="(material, i) in categoria.materiais"
      :key="i"
    >
      <img :src="material.imagem" alt="..." width="100" height="100" />
      <div class="card-body">
        <h5 class="card-title">{{ material.nome }}</h5>
        <p class="card-text">
          {{ material.descricao }}
        </p>
      </div>
      <button
        type="button"
        class="btn-success btn-sm btnreservar"
        :class="categoria.cor">Reservar</button>
    </div>
  </div>
</template>

<style>
.card-material {
  display: flex;
  flex-direction: row;
  height: 200px;
  padding: 20px;
}
.btnreservar {
  height: min-content;
  margin-top: 120px;
  color: white;
  background-color: #2b9f3f;
  border-color: #2b9f3f;
  border-radius: 5px;
}
</style>
