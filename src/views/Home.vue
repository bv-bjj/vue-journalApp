<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
  </div>
  <h1>Hola Mundo</h1>
  <button @click="goToDayBook" class="btn btn-success">Button</button>
  <button @click="goToDayBook" class="btn btn-warning">Button</button>
  <button @click="goToDayBook" class="btn btn-danger">Button</button>

</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
    
  },
  methods: {
    goToDayBook() {
      this.$router.push({  name:"no-entry"  })
    }
  }
}
</script>
