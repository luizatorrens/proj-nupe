<script>
export default {
  props: ["categoria"],
};
</script>

<template>
  <h1>{{ categoria.nome }}</h1>

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
    </div>
  </div>
</template>

<style>
.card-material {
  display: flex;
  flex-direction: row;
  height: 200px;
}
</style>
