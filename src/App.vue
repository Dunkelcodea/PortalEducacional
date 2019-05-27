<template>
  <div id="app">
    <div class="sticky-top">
  <b-navbar toggleable="lg" type="dark" variant="info">
    <b-navbar-brand href="#">Portal</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item to="/">Inicio</b-nav-item>
        <b-nav-item to="/about" >Conócenos</b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <!-- <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="Buscar"></b-form-input>
          <b-button size="sm" class="my-2 my-sm-0" type="submit">Buscar</b-button>
        </b-nav-form> -->

        <b-nav-item-dropdown text="Pendiente" right>
          <b-dropdown-item href="#">EN</b-dropdown-item>
          <b-dropdown-item href="#">ES</b-dropdown-item>
          <b-dropdown-item href="#">RU</b-dropdown-item>
          <b-dropdown-item href="#">FA</b-dropdown-item>
        </b-nav-item-dropdown>

        <b-navbar-nav right>
        <b-nav-item v-b-modal.modal-prevent-closing >Login</b-nav-item>
      </b-navbar-nav>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>
<Login/>
    <router-view/>
  </div>
</template>

<style>



#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>

<script>

import Login from '@/components/Login.vue';


export default {
  name: 'principal',
  data(){
    return{
    
    }
  },
  components: {
    Login
  }
}

</script>


