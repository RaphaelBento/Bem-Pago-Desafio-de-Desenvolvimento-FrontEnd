<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div>
 <div id="CardInteiro" >
  <div id="Cabecario">
    <img src="https://img.icons8.com/pastel-glyph/64/000000/cardboard-box.png" alt="">
        <p id="TxtHeader">Formulário para compra de</p>
  </div>
  <div id="CorpoCard">
    <span >
    <h3>Quais adesivos:</h3>
    <!-- <span style="display: flex;">
    <input type="button">
    <input type="button">
    <input type="button">
    </span> -->
    <div>
     <input type="checkbox" aria-label="Checkbox for following text input"/>
    <input type="checkbox" aria-label="Checkbox for following text input"/>
    <input type="checkbox" aria-label="Checkbox for following text input"/>
    </div>
    
    </span>
    <div class="input-group mb-3">
  <div class="input-group-prepend">
    <div class="input-group-text">
      <input type="checkbox" aria-label="Checkbox for following text input">
    </div>
  </div>
  <input type="text" class="form-control" aria-label="Text input with checkbox">
</div>
    <span id="QtdAdsivos">
        <h3>Quantos adesivos de cada ?</h3>
        <button v-on:click="Contador += 1">+</button>
        <input type="text" v-model="Contador"/>
        <button v-on:click="Contador -= 1">-</button>
         <p>Quantas vezes o botão acima foi clicado: {{ Contador }}</p>
    </span>
    <span class="EntradaDeTexto">
        <textarea class="EntradaDeTexto">
            Alguma dúvida? Recado?
        </textarea>
    </span>
  </div>
  <div id="RodaPe">
    <button type="button" class="btn btn-primary" style="background-color:#000080 ;">Enviar</button>
  </div>
  </div>
 </div>
</template>

<script>
export default {
    data(){
        return{
        nome:'Vaiavel nome',
        Contador:0
              }
          }
}
</script>

<style>
#Cabecario{
width: 100%;
    background-color: #000080;
    border-radius: 5px;
    
 
    margin-top: 10px;
        border-bottom-left-radius: 345px 37px;
    border-bottom-right-radius: 155px 85px;
}
#TxtHeader{
    color: white;
}
#CardInteiro{
    background-color: whitesmoke;
    width: 39%;
    border-radius: 5px;
    height: 500px;
    margin-left: 30%;
}
</style>