<template>
  <nav
    class="navbar navbar-expand-lg navbar-dark fixed-top flex-column"
    id="navbar"
  >
    <router-link class="navbar-brand d-flex m-auto" :to="{ name: 'Home' }">
      <div class="text-center">
        <img class="nameImg" src="../assets/name.png" alt="" />
      </div>
    </router-link>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarText"
      aria-controls="navbarText"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarText">
      <ul class="navbar-nav mr-auto text-light text-shadow">
        <a class="nav-link" href="#about"> About </a>
        <a class="nav-link" href="#skills"> Skills </a>
        <a class="nav-link" href="#portfolio"> Portfolio </a>
        <a class="nav-link" href="#contact"> Contact </a>
      </ul>
    </div>
  </nav>
</template>

<script>
import { getUserData } from "@bcwdev/auth0-vue";
import { setBearer, resetBearer } from "../services/AxiosService";
export default {
  name: "Navbar",
  methods: {
    async login() {
      await this.$auth.loginWithPopup();
      if (this.$auth.isAuthenticated) {
        setBearer(this.$auth.bearer);
        this.$store.dispatch("getProfile");
        // NOTE if you want to do something everytime the user logs in, do so here
      }
    },
    async logout() {
      resetBearer();
      await this.$auth.logout({ returnTo: window.location.origin });
    },
  },
};
</script>

<style>
.text-shadow {
  text-shadow: 1px 1px black;
}
.nameImg {
  max-height: 40px;
}
</style>
