#### Operadores Lógicos

Símbolos especiais para realizar comparações entre determinados operandos e logo retornar um resultado.

###### Tipos

* Conjunção
  
  * Só é verdadeira quando ambos os operandos são verdadeiros
  
  * Terminologia "E": expressão 1 E expressão 2.
  
  * Em Java: &&

* Disjunção
  
  * Só é falsa quando ambos os operandos são falsos
  
  * Terminologia "OU": expressão 1 OU expressão 2
  
  * Em Java: ||

* Disjunção exclusiva
  
  * Só é verdade quando ambos são opostos (V e F)
  
  * Terminologia "xor": expressão 1 xor expressão 2
  
  * Em Java: ^

* Negação
  
  * Inverte o valor lógico de um operando ou expressão
  
  * Terminologia: inversão
  
  * Em Java: !

###### Boas Práticas

Criar variáveis auxiliares para resultados intermediários, por exemplo:

> (salarioMensal < mediaSalario) && (quantidadeDependentes >= mediaDependentes)

Com auxiliares:

> (salarioBaixo) && (muitosDependentes)

> boolean recebeAuxilio =
> (salarioBaixo) && (muitosDependentes)



###### Operações bitwise e shift

Não são operadores lógicos, não confundir

Bitwise: & e |

Shift: ~, >> , >>>, <<

---

#### Controle de Fluxo

Estruturas para direcionar o fluxo de execução do código

###### Tipos

* Decisão
  
  * If
  
  * if-else
  
  * if-else-if
  
  * switch
  
  * ternário

* Repetição
  
  * for
  
  * while
  
  * do while

* Interrupção
  
  * break
  
  * continue
  
  * return

##### Decisão

Avalia uma condição booleana ou variável para direcionar o fluxo

Exemplos IF / IF - ELSE

> if (condição 1){ 
> 
> comportamento 1}

> if (condição 1){ 
> 
> comportamento 1} else {
> 
> comportamento 2 }

> if (condição 1){
> 
> comportamento 1} else if (condição 2){
> 
> comportamento 2} else {
> 
> comportamento 3}

Exemplo Ternário:

> (condição) ? (executar se true) : (executar se false)

> (condição) ? (executar se true) : null (não executa nada se false)

Exemplo Switch:

> switch (variável){
> 
> case 1:
> 
>     break;
> 
> case 2:
> 
>     break;
> 
> case...
> 
>     break;
> 
> default:
> 
>     break;
> 
> }

###### Boas práticas de fluxo

* Switch é melhor para utilizar com valores exatos (uma variável) e if para expressões booleanas

* Evitar o uso do default do Switch para cases genéricos
  
  * Default deve ser utilizado como indicador de que o valor da variável pode estar incorreta.

* Evitar efeito "flecha" dos if's | Evitar muitos if's aninhados
  
  * Utilizar as opções de else if ou switch para não deixar o if ficar muito grande e de difícil leitura


