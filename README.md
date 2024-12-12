# Joga da velha com IA
O programa implementa um jogo da velha que tem como adversário uma IA e a ideia principal é que o jogador não consiga vencer essa IA.

## 📂 Organização
-  **include:** Contém os arquivos de cabeçalho (.h) com as declarações de funções.
-  **src:** Contém os arquivos fonte (.c) com a implementação das funções.
-  **bin:** Contém o arquivo executável.
-  **Makefile:** Arquivo de configuração para a compilação.
---

## 🧠 Lógica da Inteligência Artificial
1. **Bloqueio ou Vitória imediata**:  
   - Se você ou a IA tiver duas marcações em sequência, a IA preenche o terceiro quadrado.  
   - Exemplo:  
     ```
     X | X |  
     ---------
       | O |  
     ---------
       |   |  
     Resposta da IA: 0 2
     ```  
2. **Criação de vantagens**:  
   - A IA prioriza jogadas que criem duas sequências de vitória possíveis.  
3. **Controle do centro**:  
   - A IA joga no quadrado central, se disponível.  
4. **Marcação oposta**:  
   - Se o jogador marcar um canto, a IA marca o canto oposto.  
5. **Uso de cantos vazios**:  
   - A IA preenche um canto livre antes de outras áreas.  
6. **Marcação arbitrária**:  
   - Em último caso, a IA marca qualquer quadrado vazio.

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
