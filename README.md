# Joga da velha com IA


## 📂 Organização
-  **include:** Contém os arquivos de cabeçalho (.h) com as declarações de funções.
-  **src:** Contém os arquivos fonte (.c) com a implementação das funções.
-  **bin:** Contém o arquivo executável.
-  **Makefile:** Arquivo de configuração para a compilação.
---

## 🖥️ Compilação e Execução

### Compilar
```
make
```
---
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
