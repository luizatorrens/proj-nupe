<script>
import CardCategoria from "@/components/CardCategoria.vue";

export default {
  components: { CardCategoria },
  data() {
    return {
      categorias: [
        {
          nome: "Bolas",
          cor: "verde",
          materiais: [
            {
              nome: "Bola Basquete",
              descricao: "Quantidade disponível:",
              imagem: new URL("./imgs/bbasquete.jpg", import.meta.url).href,
            },
            {
              nome: "Bola Futebol",
              descricao: "Quantidade disponível:",
              imagem: new URL("./imgs/bfutebol.png", import.meta.url).href,
            },
            {
              nome: "Bola Vôlei",
              descricao: "Quantidade disponível:",
              imagem: new URL("./imgs/bvolei.png", import.meta.url).href,
            },
          ],
        },
        {
          nome: "Tabuleiros",
          cor: "roxo",
          materiais: [
            {
              nome: "Ludo",
              descricao: "Quantidade disponível:",
              imagem: new URL("./imgs/ludo.jpg", import.meta.url).href,
            },
            {
              nome: "Xadrez",
              descricao: "Quantidade disponível:",
              imagem: new URL("./imgs/xadrez.jpg", import.meta.url).href,
            },

            {
              nome: "Banco Imobiliário",
              descricao: "Quantidade disponível:",
              imagem: new URL("./imgs/bancoimobiliario.png", import.meta.url)
                .href,
            },
          ],
        },
        {
          nome: "Cartas",
          materiais: [
            {
              nome: "Truco",
              descricao: "Quantidade disponível:",
              imagem: new URL("./imgs/truco.jpg", import.meta.url).href,
            },
            {
              nome: "Uno",
              descricao: "Quantidade disponível:",
              imagem: new URL("./imgs/uno.png", import.meta.url).href,
            },
            {
              nome: "Tradicional",
              descricao: "Quantidade disponível:",
              imagem: new URL("./imgs/baralho.png", import.meta.url).href,
            },
          ],
        },
      ],
    };
  },
};
</script>

<template>
  <CardCategoria
    v-for="(categoria, i) in categorias"
    :key="i"
    :categoria="categoria"
  />
</template>
