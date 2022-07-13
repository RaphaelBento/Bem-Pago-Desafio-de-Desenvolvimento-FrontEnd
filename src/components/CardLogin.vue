<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div>
 
  <div id="CardDemo">
    <img src="https://img.icons8.com/pastel-glyph/64/000000/cardboard-box.png" alt="">
<p id="TxtHeader">Formulário para compra de</p>
  </div>
  
 </div>
</template>

<script>
export default {
    data(){
        return{
        nome:'Vaiavel nome'
              }
          }
}
</script>

<style>
#CardDemo{
width: 30%;
    background-color: #000080;
    border-radius: 5px;
    position: relative;
    left: 30%;
    margin-top: 10px;
        border-bottom-left-radius: 345px 37px;
    border-bottom-right-radius: 155px 85px;
}
#TxtHeader{
    color: white;
}
</style>