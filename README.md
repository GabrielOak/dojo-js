# Dojo - JavaScript

## Declaração de Váriavel

```` javascript
    var x = 0; // Pode ser usada fora do escopo da função
    let y; //  Fica limitada a o escopo da função (é a melhor opção)
    const k; // Não pode ter o seu valor alterado

````

## Operações

``` javascript

    10 + 10 // adição
    12 - 5 // subtração
    15 * 3 // multiplicação
    10 / 2 // divisão
    10 % 2 // Módulo da divisão -> resto da divisão
    3 ** 3 // Potenciação
    x++ // Incremento -> x = x + 1
    y-- // Decremento -> y = y - 1

    // Também aceita operações como:
    x+=5 // x = x + 5
    x-=2 // x = x - 2
    x*=4 // x = x * 4
    x/=2 // x = x / 2
    x%=2 // x = x % 2
    x**=3 //x = x ** 3

```


##  Comparações 

``` javascript
    2 == 2 // igual 
    5 === 5 // valor igual e tipo igual
    2 != 6 // diferente
    5 > 2 // maior que
    2 < 5 // menor que
    5 >=2 // maior igual
    2 <= 5 // menor igual

```

## Operações Lógicas

``` javascript

    true && false // and 
    false || false // or
    !false // not 

``` 

## Tipos

``` javascript

    let idade = 33 // Number 
    const nome = 'José' // String
    const info = {nome: "Jose", idade: 33 } // Object

    typeof(1.2) // number
    typeof("Dojo") // string
    typeof([1, 2, 3]) // object
    typeof(false) // boolean

```

## String

``` javascript

    let dojo = "Dojo"
    let js = "JavaScript"
    let nome = dojo + "de" + js // Dojo de JavaScript
    let nome = `${dojo} de ${js}` // Dojo de JavaScript 

    nome.length // Retorna o tamanho da string - 18
    nome.indexOf("de") // Retorna o index primeira ocorrência da string - 5
    nome.lastIndexOf("de") // Retorna o index da ultma occorência da string - 5
    nome.replace("Dojo", "de") // Dojo Dojo JavaScript
    nome.toUpperCase() // DOJO DE JAVASCRIPT
    nome.toLowerCase() // dojo de javascript
    nome.trim() // Remove espaço no inicio e fim da string 

```
[Link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) para saber mais sobre strings em JS. 

## Array

``` javascript

    const lista = ['batata', 'leite', 'pão']
    lista[0] // batata 
    lista[1] = 'soja' 
    lista.length // 3
    lista.push('limão') // Adiciona um elemento ao final do array
    lista.pop() // Remove o ultimo elemento do array 
    lista.shift() // Remove o primeiro elemento do array
    lista.unshift("laranja") // Adiciona um elemento no inicio do array
    lista.sort() // Ordena o array 
    lista.reverse() // Odernao o array da maneira inversa 


```

## Condicional

``` javascript

    if(condição){
        // ...
    } else if(outra condição){
        // ...
    }else{
        // ...
    }

    switch(frutas){
        case "batata":
            // faz algo
            break;
        case "maçã":
            // faz algo
            break;
        default:
            // faz algo
    } 

    // Operador ternário

    // condicao? verdadeira : falsa
    5 > 2? 'maior' : 'menor' // retorna maior
    5 > 7? 'maior' : 'menor' // retorna menor

```
## Loop

``` javascript

    for(let i=0; i<10; i++){
        // faz algo 
    }

    while(condição){
        // faz algo
    }

    const lista = ['maçã', 'banana', 'melão']
    for(fruta in lista){
        console.log(fruta)
    }

    lista.map((fruta) =>{
        console.log(fruta) 
    }) 

``` 

## Função

``` javascript

    function sum(x, y){
        return x + y
    } 

    const sum = (x,y) => {
        return x + y
    }

    const sum = (x, y) => x + y // return implícito 

``` 

## Objeto

``` javascript

    const ayrton = {
        nome: "Ayrton",
        sobrenome: "Senna",
        idade: 34,
        profissao: "piloto",
        nomeCompleto: function (){
            return this.nome + " " + this.sobrenome
        },
    }

``` 

## Classe

``` javascript

    class Pessoa{

        constructor(nome, sobrenome, idade, profissao){
            this.nome = nome
            this.sobrenome = sobrenome
            this.idade = idade
            this.profissao = sobrenome
        }
        
        nomeCompleto(){
            return `${this.nome} ${this.sobrenome}`
        }
    }

    let pedro = new Pessoa('Pedro', 'Alves', 22, 'Jornalista');

```
