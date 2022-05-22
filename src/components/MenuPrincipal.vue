<template>
  <div class="collapse bg-light" id="navbarHeader">
    <div class="container">
      <div class="row">
        <div class="col-sm-8 col-md-7 py-4">
          <h4 class="text-success">Sobre</h4>
          <p class="text-muted">
            Este site é voltado para o empréstimo de materiais disponibilizados pelo NUPE. Para realizar o empréstipo é necessário fazer o cadastro.
          </p>
        </div>
        <div class="col-sm-4 offset-md-1 py-4">
          <br />
          <ul class="list-unstyled">
            <li>
              <a href="#" class="text-success">Contato</a>
            </li>
            <li>
              <a href="#" class="text-success"
                >Cadastre-se!</a
              >
            </li>
            <li><a href="#" class="text-success">Logar</a></li>
          </ul>
        </div>
      </div>
    </div>
    <hr>
  </div>

  <div class="navbar navbar-dark bg-light shadow-sm col-12 col-sm-11">
    <a href="#" class="navbar-brand d-flex align-items-center">
      <img
        class="logo"
        src="../components/imgs/logoifc.png"
        alt=""
        height="100px"
        width="130px"
      />
    </a>

    <button
      class="navbar-toggler buttonnav"
      type="button"
      data-bs-toggle="collapse"
      data-bs-target="#navbarHeader"
      aria-controls="navbarHeader"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
  </div>
</template>
