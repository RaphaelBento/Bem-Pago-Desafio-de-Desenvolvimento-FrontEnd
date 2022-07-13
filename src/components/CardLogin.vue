<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div>
 <div id="CardInteiro" >
  <div id="Cabecario">
       <img src="../assets/CaixaBox.png" alt="Imagem CardBoardBox"/>
       <p id="TxtHeader">Formulário para compra de</p>
  </div>
  <div id="CorpoCard">
   
    <h5>Quais adesivos:</h5>
    
    <div class="form-check">
    <input type="checkbox" class="form-check-input" />
     <label class="form-check-label" for="exampleRadios1">
    React
  </label>
    </div>
    <div class="form-check">
    <input type="checkbox" class="form-check-input"/>
    <label class="form-check-label" for="exampleRadios1">
    Vue
   </label>
</div>
    <div class="form-check">
    <input type="checkbox" class="form-check-input"/>
    <label class="form-check-label" for="exampleRadios1">
    Angular
    </label>
    </div>
    
    <span id="QtdAdsivos">
        <h5>Quantos adesivos de cada ?</h5>
        <button v-on:click="Contador += 1" style="background-color: #2f3675;">+</button>
        <input type="text" v-model="Contador" id="DisplayContador"/>
        <button v-on:click="Contador -= 1" style="background-color:#2f3675;">-</button>
         <p>Quantas vezes o botão acima foi clicado: {{ Contador }}</p>
    </span>
    <div class="" id="EntradaTxt">
        <h5 id="TitleObser">Observações:</h5>
      <textarea  class="form-control" id="AreaTxt">
            Alguma dúvida? Recado?
        </textarea>
    </div>
  </div>
  <div id="RodapeBtn">
    <button type="button" class="btn btn-primary" id="BtnEnviar">Enviar</button>
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
    background-color: #2e3675;
    border-radius: 5px;
    
 
    margin-top: 10px;
        border-bottom-left-radius: 345px 37px;
    border-bottom-right-radius: 155px 85px;
}
#TxtHeader{
    color: white;
}
#CardInteiro{
    background-color:#f2f2f2;
    width: 29%;
    border-radius: 5px;
    height: 750px;
    margin-left: 30%;
}
#DisplayContador{
    background-color: #F5F5F5;
}
#AreaTxt{
    background-color: #dde3e9;  
    width: 86%;
   
    height: 178px;
}
#BtnEnviar{
    
    background-color: #000080;
    position: relative;
    left: 60%;
    width: 31%;
    margin-top: 12px;
}
#RodapeBtn{
    
    /* width: 100%;
    
    border-radius: 10px;
    height: 80px;
    margin-top: 33%; */
    background-color: #dde3e9;
    margin-top: 116px;
    height: 8%;
    border-radius: 5px;
}
#EntradaTxt{
    position: relative;
    left: 7%;
    margin-bottom: 11%;
}
</style>