# Simulador de Loteria

Este projeto é um simulador da *megasenna*, onde o usuário digita seis numeros.
E sorteamos aleatoriamente outros seis numeros e comparamos para verificar.
quantos você acertou.

**Não é para jogos oficiais**

## Tecnologias utilizadas
1. **HTML**: HTML é uma linguagem de marcação
utilizada na construção das estruturas das páginas
na web.
2. **CSS**: Cascading Style Sheets (CSS) é um
mecanismo para adicionar estilo (cores, fontes,
espaçamento, etc.) a um documento web
3. **JS**: JavaScript (frequentemente abreviado
como JS) é uma linguagem de programação
interpretada estruturada, de script em alto nível
com tipagem dinâmica fraca e multiparadigma
(protótipos, orientado a objeto, imperativo e, funcional).
4. ~~**Jquery**~~: Não foi utilizado.

## Funções Principais
Aqui será apresentado as duas funções principais do site.

### Sorteio de numeros
Nessa função os numeros são sorteados aletoriamente
```
function sortear(){
	numSort = [];
	for (var i = 0; i < 6; i++) {
		do{
			sort = Math.ceil(Math.random()*60)
			if(sort == 0){
			sort++;
			}
		}while(numSort.includes(sort));
		numSort.push(sort);
	}
	console.log(numSort);
}
```

### Lendo os Numeros digitados
Lê as entradas de numeros digitadas pelo usuário
```
function addList(num, pos){
	if(num.length == 2){
		if(numEsco.includes(num)){
		alert("Numero ja escolhido");
		}else if(parseInt(num) > 60){
			alert("O numero inserido não pode ser maior que 60");
		}
		else{
			numEsco[pos-1] = num;
		}
	}
}
```

## Como rodar o código
> Simplesmente baixe o código e abra o arquivo **_index.html_** no seu navegador
