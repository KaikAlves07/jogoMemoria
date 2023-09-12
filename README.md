# jogoMemoria
Esse repositorio tem um jogo muito louco da memoria

2023-09-11
-Criação do index.html
-Criação do script.js
const entrada = document.getElementById("entrada");
const btn = document.getElementById("btn");

let NumSecreto = Math.random()*100;
NumSecreto = Math.round(NumSecreto)
let erro = 0

btn.addEventListener("click" , function(){
    console.log(entrada.value)
    //verfico se o valor de entrada é o número correto

    if(entrada.value < NumSecreto){
        alert("O numero secreto é maior")
        erro = erro + 1;
    }else if(entrada.value > NumSecreto){
        alert("O numero secreto é menor")
        erro = erro + 1;
    }else{
        alert("Você acertou depois de " + erro + " erros")

    }
})
