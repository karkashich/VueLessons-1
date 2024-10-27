<template>
  <h3>{{info}}</h3>
  <p>{{someInfo}}</p>
  
  <button  type="button" @click="userData()"></button>
  <button  type="button" @mouseenter="userData()"></button>
</template>

<script>
 export default{
    data(){
      return {
        info: "кнопка ни разу не нажималась",
        someInfo: "Нижмите на кнопку ниже"
      }
    },
    methods:{
      userData(){
        this.info = 'Кнопка была нажата'
        this.someInfo = 'Вы навелись на кнопку'
      }
    }
 }
</script>

<style scoped>
    h3{
      font-weight: 300;
    }
    p{
      color: blueviolet;
    }
    button{
      width: 200px;
      height: 50px;
    }
</style>

