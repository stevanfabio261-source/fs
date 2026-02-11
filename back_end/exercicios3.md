exercicios1
for (let i = 6; i <= 11; i++) {
    process.stdout.write(i + " ");
}console.log("Acabou!)


exercicios2
for (let i = 10; i >= 3; i--) {
    process.stdout.write(i + " ");
}

console.log("Acabou!");

exercicios3
for (let i = 0; i <= 18; i += 3) {
    process.stdout.write(i + " ");
}

console.log("Acabou!");

exercicios4

for (let i = 100; i >= 0; i -= 5) {
    process.stdout.write(i + " ");
}
console.log("Acabou!");

exercicios5
const readline = require("readline-sync");

let valor = parseInt(readline.question("Digite um valor inteiro e positivo: "));

for (let i = 1; i <= valor; i++) {
    process.stdout.write(i + " ");
}
console.log("Acabou!");

exercicios6
for (let i = 30; i >= 1; i--) {
    if (i % 4 === 0) {
        process.stdout.write("[" + i + "] ");
    } else {
        process.stdout.write(i + " ");
    }
}
exercicios7
const readline = require("readline-sync");

let inicio = parseInt(readline.question("Primeiro valor: "));
let fim = parseInt(readline.question("Ultimo valor: "));
let incremento = parseInt(readline.question("Incremento: "));

for (let i = inicio; i <= fim; i += incremento) {
    process.stdout.write(i + " ");
}
console.log("Acabou!");

exercicios8
if (inicio < fim) {
    for (let i = inicio; i <= fim; i += incremento) {
        process.stdout.write(i + " ");
    }
} else {
    for (let i = inicio; i >= fim; i -= incremento) {
        process.stdout.write(i + " ");
    }
}
console.log("Acabou!");

exercicios9
let soma = 0;

for (let i = 6; i <= 100; i += 2) {
    soma += i;
}

console.log("Soma =", soma);

exercicios10
let soma = 0;

for (let i = 500; i >= 0; i -= 50) {
    soma += i;
}

console.log("Resultado =", soma);

exercicios11
let soma = 0;

for (let i = 1; i <= 7; i++) {
    let num = parseInt(readline.question("Digite um numero: "));
    soma += num;
}

console.log("Somatorio =", soma);

exercicios12
let pares = 0;
let impares = 0;

for (let i = 1; i <= 6; i++) {
    let num = parseInt(readline.question("Digite um numero: "));
    
    if (num % 2 === 0) {
        pares++;
    } else {
        impares++;
    }
}

console.log("Pares:", pares);
console.log("Impares:", impares);

exercicios13
let acima5 = 0;
let div3 = 0;

for (let i = 1; i <= 20; i++) {
    let num = Math.floor(Math.random() * 11);
    process.stdout.write(num + " ");
    
    if (num > 5) acima5++;
    if (num % 3 === 0) div3++;
}

console.log("\nAcima de 5:", acima5);
console.log("Divisiveis por 3:", div3);

exercicios14
let maior = 0;
let menor = Infinity;

for (let i = 1; i <= 8; i++) {
    let preco = parseFloat(readline.question("Preco: "));
    
    if (preco > maior) maior = preco;
    if (preco < menor) menor = preco;
}

console.log("Maior preco:", maior);
console.log("Menor preco:", menor);

exercicios15
let soma = 0;
let maiores18 = 0;
let menores5 = 0;
let maiorIdade = 0;

for (let i = 1; i <= 10; i++) {
    let idade = parseInt(readline.question("Idade: "));
    
    soma += idade;
    if (idade > 18) maiores18++;
    if (idade < 5) menores5++;
    if (idade > maiorIdade) maiorIdade = idade;
}

console.log("Media:", soma / 10);
console.log("Maiores de 18:", maiores18);
console.log("Menores de 5:", menores5);
console.log("Maior idade:", maiorIdade);

exercicios16
let homens = 0;
let mulheres = 0;
let soma = 0;
let somaHomens = 0;
let mulheres20 = 0;

for (let i = 1; i <= 5; i++) {
    let idade = parseInt(readline.question("Idade: "));
    let sexo = readline.question("Sexo (M/F): ");
    
    soma += idade;
    
    if (sexo.toUpperCase() === "M") {
        homens++;
        somaHomens += idade;
    } else {
        mulheres++;
        if (idade > 20) mulheres20++;
    }
}

console.log("Homens:", homens);
console.log("Mulheres:", mulheres);
console.log("Media grupo:", soma / 5);
console.log("Media homens:", somaHomens / homens);
console.log("Mulheres > 20:", mulheres20);

exercicios17
let homens = 0;
let mulheres = 0;
let soma = 0;
let somaHomens = 0;
let mulheres20 = 0;

for (let i = 1; i <= 5; i++) {
    let idade = parseInt(readline.question("Idade: "));
    let sexo = readline.question("Sexo (M/F): ");
    
    soma += idade;
    
    if (sexo.toUpperCase() === "M") {
        homens++;
        somaHomens += idade;
    } else {
        mulheres++;
        if (idade > 20) mulheres20++;
    }
}

console.log("Homens:", homens);
console.log("Mulheres:", mulheres);
console.log("Media grupo:", soma / 5);
console.log("Media homens:", somaHomens / homens);
console.log("Mulheres > 20:", mulheres20);

exercicios18
let secreto = Math.floor(Math.random() * 10) + 1;
let acertou = false;

for (let i = 1; i <= 4; i++) {
    let palpite = parseInt(readline.question("Tentativa " + i + ": "));
    
    if (palpite === secreto) {
        console.log("Voce acertou!");
        acertou = true;
        break;
    } else {
        console.log("Errou!");
    }
}

if (!acertou) {
    console.log("Suas tentativas acabaram! O numero era", secreto);
}

