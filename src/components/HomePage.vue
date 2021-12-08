<template>
  <section class="home">
    <a class="logo">Malangas</a>
    <div class="description">
      <h1>JEWELLRY</h1>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci,
        dolorem suscipit neque saepe voluptas aliquid.
      </p>
      <button v-on:click="sendToLogIn">
        <ges-icon icon="sign-in-alt" size="lg" />
        Iniciar Sesión
      </button>
      <button v-on:click="sendToSignUp">
        <ges-icon icon="sign-in-alt" size="lg" />
        Registrarse
      </button>
    </div>
    <img src="../assets/img/home.jpg" />
    <div class="social-container">
      <ul class="social-icons">
        <li>
          <a href="#"><i class="fa fa-facebook"></i></a>
        </li>
        <li>
          <a href="#"><i class="fa fa-instagram"></i></a>
        </li>
      </ul>
    </div>
  </section>
  <footer class="footer">
    <a class="logo">Malangas</a>
    <div class="contact">
      <h3>+000000000</h3>
      <p>Todos los derechos reservados</p>
    </div>
  </footer>
</template>
<script>
export default {
  name: "homePage",
  data: () => {
    return {
      modules: [
        {
          title: "Proveedores",
          description:
            "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et",
        },
        {
          title: "Usuarios",
          description:
            "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et",
        },
        {
          title: "Productos",
          description:
            "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et",
        },
      ],
    };
  },
  methods: {
    sendToLogIn: function () {
      this.$router.push({ name: "logIn" });
    },
    sendToSignUp: function () {
      this.$router.push({ name: "signUp" });
    },
  },
};
</script>