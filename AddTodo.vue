<template>
  <form>
      <b-input v-model="name" placeholder="unesi email za registraciju u profil"></b-input>
        
      <b-button >Registriraj se</b-button>
  </form>
</template>

<script>
export default {
    data (){
        return{
        }
    }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
   form{
       display:flex;
       margin-top: 20px;
       padding-top: 2px;
       border-top: 1px solid #EFEFEF;
   }
   div{
       flex:1;
       margin-right: 20px;
   }
    button{
        margin-top: auto;
    }
</style>
