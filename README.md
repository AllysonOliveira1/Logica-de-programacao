alert('Bem vindo ao jogo do numero secreto');
let numeroMaximo = 2000
let numeroSecreto = parseInt(Math.random() *numeroMaximo + 1);
console.log(numeroSecreto);
let chute;
let tentativas = 1;

while(numeroSecreto != chute){
    chute = prompt('Escolha um número entre 1 e ' +numeroMaximo);

    if(numeroSecreto == chute) {
        break;
    } else{
        if(chute > numeroSecreto){
            alert('Numero secreto é menor que ' +chute);
        }else{
                alert('Número secreto é maior que ' +chute);
            }
        tentativas++;
    }

}
let palavraTentativa = tentativas > 1 ? 'tentativas' : 'tentativa'
alert(`Você descobriu o número secreto ${numeroSecreto} com ${tentativas} ${palavraTentativa}`);
