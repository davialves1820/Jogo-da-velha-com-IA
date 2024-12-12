# Joga da velha com IA
O programa implementa um jogo da velha que tem como adversário uma IA e a ideia principal é que o jogador não consiga vencer essa Ia.

## 📂 Organização
-  **include:** Contém os arquivos de cabeçalho (.h) com as declarações de funções.
-  **src:** Contém os arquivos fonte (.c) com a implementação das funções.
-  **bin:** Contém o arquivo executável.
-  **Makefile:** Arquivo de configuração para a compilação.
---

## Lógica por trás da Ia
A lógica por trás do comportamente da IA segue 6 regras simples que devem ser seguidas nessa ordem:

- Se você ou seu oponente tiver duas marcações em sequência, marque o 
quadrado restante.
- Se houver uma jogada que crie duas sequências de duas marcações, 
use-a.
- Se o quadrado central estiver livre, marque-o. 
- Se seu oponente tiver marcado um dos cantos, marque o canto oposto.
- Se houver um canto vazio, marque-o.
- Marque arbitrariamente um quadrado vazio.

Com isso, se espera que a IA se torne invencível contra o jogador.

## 🖥️ Compilação e Execução

### Compilar
```
make
```

### Executar
```
./bin/programa
```
---

## 🎮 Como Jogar

Quando o jogo começar, o tabuleiro será exibido com coordenadas para as linhas e colunas:

```
colunas     0   1   2       linhas

             |   |           0
         ------------
             |   |           1
         ------------
             |   |           2
```
O jogador deve digitar a linha e a coluna onde deseja jogar. Exemplo:

```
digite a linha e coluna que voce quer jogar(nessa ordem): 1 1
```
O tabuleiro será atualizado automaticamente após cada jogada.

O jogo termina quando:
- Um dos jogadores vencer.
- Todas as posições forem preenchidas (empate).

---
