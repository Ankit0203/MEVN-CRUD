<template>
<div>
   <b-navbar type="dark" variant="dark">
    <b-navbar-nav>
      <b-nav-item><router-link to="/">Home</router-link></b-nav-item>
      <b-nav-item><router-link to="/table">Table</router-link></b-nav-item>
      <b-nav-item><router-link to="/about">About</router-link></b-nav-item>

    </b-navbar-nav>
  </b-navbar>
  </div>
</template>

<script>
export default {
    name : "Header"
}
</script>
