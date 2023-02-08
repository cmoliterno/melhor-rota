# Melhor Rota

Projeto produzido utilizando Python para escolher a melhor rota entre Origem e Destino com o menor custo de percurso.


## Requisitos
- Python 3.6+

## Clonar projeto
```bash
git clone https://github.com/cmoliterno/melhor-rota.git
```
--
## Intalação de bibliotecas:
1. Tkinter
>  pip install tk-tools

2. SimpleGUI
>  pip install PySimpleGUI
--
## Executando a aplicação
1. Após clonar o projeto, acesse a pasta raiz do projeto
3. Execute o arquivo Main.py pelo terminal:
  > python May.py
 
## Aplicação
1. Após executar o comando anterior, deverá ser exibido uma  tela com a inteface gráfica da aplicação.

<p align="center">
    <img src="/Interface Gráfica.png">
</p>
2. Informe o nome contindo dentro de um local (letra indicada. Ex "A") no campo de origem
3. Informe o nome contindo dentro de um local (letra indicada. Ex "A") no campo de destino
4. Pressione em enviar.
5. A melhor rota deverá ser traçada em verde e o Km total será exibido no canto inferior direito da aplicação.
6. Repita o processo para mais testes.

## Validação
1. Para validar se a rota traçada é a melhor, basta somar os números presente nas semi-retas que podem ser traçadas saindo da origem e chegando no destino

## Objetivo
Após uma pré carga/configuração de dados para validação, temos o mapeamento dos locais e a distância em KM entre cada local:

# Locais

<p align="center">
    <img src="/Locais Registrados.png">
</p>

# Distância

<p align="center">
    <img src="/KM da Rota.png">
</p>

## Algoritmo
1. O caminho é traçado utilizando a busca de custo uniforme, que possui como g(x) os custos presentes nas semi-retas, importantes para traçar a solução ótima, neste caso.
2. Para conseguir o caminho percorrido para chegar ao destino, cada nó que é expandido possui uma lista que contém todos os nós que foram visitados para que pudesse chegar até ali.
Ou seja, cada um possui uma lista propria do caminho percorrido até o momento da expansão daquele nó.

<p align="center">
    <img src="/Algoritmo para calcular a melhor rota com menor km percorrida.png">
</p>

3. Após aplicação do algoritmo a melhor rota é identificada:

<p align="center">
    <img src="/Melhor Rota Identificada.png">
</p>

4. Existe a possibilidade de elevar a complexidade incluindo informações de tráfico ao algoritmo elevando sua eficiência máxima com relação a redução de custos


## Autor
- Caroline Moliterno