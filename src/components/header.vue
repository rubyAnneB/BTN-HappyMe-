<template>
  <div> 
    <a href="" @click.prevent="logout">Logout</a>
  </div>
</template>
<script>
  export default {
    methods: {
      logout(){
        localStorage.removeItem('token');
        this.$router.push('/login');
      }
    }
  }
</script>