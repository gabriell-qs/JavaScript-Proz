# JavaScript - Proz
Exercícios realizados durante a disciplina 'Linguagem de Programação', ministrada no curso de _Desenvolvimento de Sistemas_ da Escola Proz

<hr>

### **Variáveis, Operadores Aritméticos, Concatenação, Relacionais e Lógicos - parte 1**

**Q1.** Crie um programa cujo objetivo é inserir seus dados pessoais (nome, idade, gênero e cidade) e armazenar em cada variável determinada e depois exibidos na tela.
```
var nome = ""
var idade = ""
var genero = ""
var cidade = ""


nome = prompt("digite seu nome: ")

document.write("<br>ola " + nome + " seja bem vindo! ")

idade = prompt("digite sua idade: ")

document.write("<br>voce tem " + idade + " anos! ")

genero = prompt("digite seu genero: ")

document.write("<br>voce é " + genero )

cidade = prompt("digite sua cidade: ")

document.write("<br>voce é de " + cidade  )
```
**Q2.** Dado o cálculo 12 x 3 + 4 - 8 / 2 % 3, qual o resultado segundo a precedência de operadores?
```
var numero = (12 * 3) + 4 - (8 / 2) % 3

document.write("<br> o  resuitado de 12 * 3 + 4 - 8 / 2 % 3 é : " + numero )

document.write(" O resultado da expressão 12 * 3 + 4 - 8 / 2 % 3 é: " + calculo)
```
**Q3.** Crie um programa que utilize os métodos de Strings, onde o usuário envia uma frase e o programa exibe as informações dessa frase (tamanho, letra maiúscula, letra minúscula, substring e index).
```
var texto = ""
var letra = ""
var achar = texto.indexOf(letra)

texto = prompt("qual a frase?")
document.write("<br>a frase é :" + texto )
document.write("<br>o  tamanho é :" + texto.length )
document.write("<br>a frase cortado :" + texto.substring(0,9) )
document.write("<br>em forma maiuscula :" + texto.toUpperCase() )
document.write("<br>em forma mininuscula :" + texto.toLowerCase() )

letra = prompt("qual a letra que voce quer achar?")

if(achar){ 
    document.write("<br> a frase tem a " + letra + " na " + texto)

}else {
    document.write("<br> a "+ texto + " nao tem a letra " + letra)
}

```
### **Variáveis, Operadores Aritméticos, Concatenação, Relacionais e Lógicos - parte 2**

**Q1.** Crie um programa que peça ao usuário para inserir dois números. Verifique se eles são iguais e exiba uma mensagem indicando o resultado.
```
var num1 = ""
var num = ""
num1 = prompt("digite um numero:")

num = prompt("agora, digite outro numero:")

document.write("<br> 0  numero 1 e: " + num1 + "  numero  2 e : " + num)

if(num1 == num){
    document.write("<br> vc tem dois numeros iguais")
}else{
    document.write("<br>vc nao ten numeros iguais")
}

```
**Q2.** Crie um programa que peça ao usuário para inserir dois números. Verifique se eles são pares e exiba uma mensagem indicando o resultado.
```
var numero =  prompt("<br>digite o numero")
var numero2 = prompt("<br>digiete o segundo numero")


if(numero % 2 == 0){
    document.write("<br>seu  primeiro numero é par")
}else{
document.write("<br>seu primeiro numero nao e par")
}


if(numero2 % 2 == 0){
document.write("<br>seu segundo numero é par")
}else{
document.write("<br>seu segundo numero nao e par")
}
```
**Q3.** Crie um programa que peça ao usuário para inserir dois números. Verifique se eles são ímpares e exiba uma mensagem indicando o resultado.
```
var numero = 0
var numero2 = 0
numero = prompt("<br>digite o numero")
numero2 = prompt("<br>digiete o segundo numero")


if(numero % 2 == 0 ){
    document.write("<br>seu primeiro numero nao e impar")
}else{
document.write("<br>seu primeiro numero e impar")
}

if(numero2 % 2 == 0) {
    document.write("<br>seu segundo numero nao e impar ")
}else{
document.write("<br>seu segundo numero e impar ")
}
```
**Q4.** Crie um aplicativo que calcule o Índice de Massa Corporal (IMC) de uma pessoa. Peça o peso e a altura, e calcule o IMC usando a fórmula: IMC = peso / (altura * altura). E por fim, indique, de acordo com o resultado, se a pessoa está: 
* Abaixo do normal
* Normal
* Sobrepeso
* Obesidade grau I
* Obesidade grau II
* Obesidade grau III
```
var peso = 0
var tamanho = 0
peso = prompt("<br>digite seu peso")
tamanho = prompt("<br>digite seu tamanho")

document.write("<br>seu peso é " + peso)
document.write("<br>seu tamanho é " + tamanho)

var imc = peso/(tamanho*tamanho)

if(imc<18.5){
    document.write("<br> abaixo do normal")
}else if(18.5 <imc< 24.9){
    document.write("<br>normal")
}else if(25< imc <29.9){
    document.write("<br>sobrepeso")
}else if(30< imc <34.9){
    document.write("<br>obesidade grau 1")
}else if(35< imc <39.9){
    document.write("<br>obesidade grau 2")
}else {
    document.write("<br>obesidade grau 3")
}
```
**Q5.** Desenvolva um jogo interativo de pedra, papel e tesoura onde o usuário pode competir contra o computador. Dica: utilize o método de Matemática random para criar um número aleatório.
```
var usuario = prompt("<br>escolha pedra, papel, tesoura")
usuario = usuario.toLowerCase();
var computador = Math.ceil(Math.random(0,2))

if (usuario == "papel"){
    if(computador == 2){
        document.write("ele escolheu tesoura voce perdeu")
}else if(computador == 0){
        document.write("<br>ele escolheu pedra voce venceu")
}else if(computador == 1){
        document.write("ele escolheu papel empatou ")}

}else if(usuario == "tesoura"){
if(computador == 0){
        document.write(" ele escolheu pedra voce perdeu")
}else if(computador == 1){
        document.write("<br> ele escolheu papel voce venceu")
}else if(computador == 2){
        document.write("ele escolheu tesoura empatou")}

}else if(usuario == "pedra"){
    if(computador == 1){
        document.write(" ele escolheu papel voce perdeu")
}else if(computador == 2){
        document.write("<br> ele escolheu tesoura voce vence")
}else if(computador == 0){
        document.write(" ele escolheu pedra empatou ")}
    }



```
### **Funções**

**Q1.** Para um site de e-commerce, desenvolva um programa com uma função que calcula o preço total com base na quantidade de produtos inserida pelo usuário. A entrada é recebida como uma string e precisa ser convertida em um número inteiro antes de ser multiplicada pelo preço unitário.
```
var precoU = 30.0;
var quantidadeString = prompt("digite a quantidades de produtos")
function qtotal(){

    var quant = parseInt(quantidadeString,10);



if (isNaN(quant) || quant <= 0){

    document.write("por favor,  insira uma quantidade valida");
return}


var precoT = quant*precoU;

document.write("o preço total "+quant+" produtos e:  "+ precoT.toFixed(2)) }

qtotal();
```
**Q2.** Desenvolva um programa para aplicar descontos aplicativo que ajuda os usuários a rastrear seus gastos. Como parte deste aplicativo, os usuários podem inserir o preço de um produto, o valor do desconto e o aplicativo calcula o valor total após aplicar um desconto.
```
function calD(){

    var precoOriginalString = prompt("digite o preço do produto:")

    var precO = parseFloat(precoOriginalString)

    if(isNaN(precO)||precO<=0){
        document.write("erro por favor insira um preço valido")
        return;
    }

    var descontoString = prompt("digite o desconto(%)");
    var dec = parseFloat(descontoString)

    if (isNaN(dec)|| dec < 0 || dec > 100){
document.write("erro por favor insira um desconto valido(entre 1  a 100%)")
return
    }

    var valorD = (precO*dec)/100
    var precfinal = precO-valorD

    document.write("preço original: " + precO.toFixed(2) + "<br>")
    document.write("desconto aplicado " + dec + "%<br>")
    document.write("valor do desconto: " + valorD.toFixed(2) + "<br>")
    document.write("preço final R$:" + precfinal.toFixed(2))

}

calD()
```
**Q3.** Desenvolva uma calculadora.
```
document.write("Bem-vindo à calculadora!");


var operacao = prompt("Digite a operação desejada: ");
var num1 = parseFloat(prompt("Digite o primeiro número: "));
var num2 = parseFloat(prompt("Digite o segundo número: "));

let resultado;

if (operacao === "+") {
    resultado = num1 + num2;
} else if (operacao === "-") {
    resultado = num1 - num2;
} else if (operacao === "*") {
    resultado = num1 * num2;
} else if (operacao === "/") {
    if (num2 !== 0) {
        resultado = num1 / num2;
    } else {
        document.write("Erro: Divisão por zero não é permitida.");
        process.exit(); 
    }
} else {
    document.write("Operação inválida.");
    process.exit(); 
}

document.write(`O resultado é: ${resultado}`);
```
### Laços de Repetição + Datas + POO - Programação Orientada a Objetos

**Q1.** Desenvolva um programa que informa a tabuada de um número inserido pelo usuário.
```
let numero = parseInt(prompt("Digite um número para ver sua tabuada:"));


if (isNaN(numero)) {
    alert("Por favor, insira um número válido.");
} else {

    let resultado = "";
    for (let i = 1; i <= 10; i++) {
        resultado += `${numero} x ${i} = ${numero * i}\n`;
    }
    document.write("Tabuada do " + numero + ":\n" + resultado );
}
```
**Q2.** Conforme com o que você aprendeu sobre manipulação de datas, faça as contas: quantos dias se passaram da data do seu nascimento até o dia de hoje?
```
function diasPassados(dataNascimento, dataAtual) {
    var nascimento = new Date(dataNascimento);
    var atual = new Date(dataAtual);
    
    var diffTime = atual - nascimento; 
    var diffDays = diffTime / (1000 * 3600 * 24); 
    return Math.floor(diffDays); 
}

var dataNascimento = "2005-08-03";
var dataAtual = new Date(); 


document.write(diasPassados(dataNascimento, dataAtual));
```
**Q3.** Utilizando a programação Orientada a Objetos, monte um modelo de construção de um sistema de uma das empresas abaixo: 
* Netflix
* Ifood
* Airbnb
* Uber/99
```
class Usuario {
    constructor(nome, telefone) {
    this.nome = nome;
    this.telefone = telefone;
    }

    exibirInfo() {
    document.write(`Nome: ${this.nome}, Telefone: ${this.telefone}`);
    }
}
class Motorista extends Usuario {
    constructor(nome, telefone, placaCarro) {
    super(nome, telefone);
    this.placaCarro = placaCarro;
    }
    exibirInfo() {
    super.exibirInfo();
    document.write(`Placa do carro: ${this.placaCarro}`);
    }
}
class Passageiro extends Usuario {
    constructor(nome, telefone) {
    super(nome, telefone);
    }
    avaliarMotorista() {
    document.write(`${this.nome} avaliou o motorista.`);
    }
}
class Corrida {
    constructor(motorista, passageiro, origem, destino) {
    this.motorista = motorista;
    this.passageiro = passageiro;
    this.origem = origem;
    this.destino = destino;
    }
    iniciar() {
    document.write(`Corrida iniciada de ${this.origem} para ${this.destino}.`);
    }
    concluir() {
    document.write(`Corrida concluída. ${this.origem} -> ${this.destino}`);
    }
}
    var motorista = new Motorista('Carlos Silva', '999999999', 'XYZ-1234');
    var passageiro = new Passageiro('João Pereira', '888888888');
motorista.exibirInfo();
passageiro.exibirInfo();
    var corrida = new Corrida(motorista, passageiro, 'Av. Paulista', 'Itaim Bibi');
corrida.iniciar();
corrida.concluir();
passageiro.avaliarMotorista();
```
