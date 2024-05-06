# Análise Hierárquica de Tarefas (HTA)

## Introdução
A Análise Hierárquica de Tarefas (HTA) é uma metodologia desenvolvida na década de 1960, com o intuito de compreender a execução de tarefas complexas e não repetitivas, examinando primeiramente objetivos de alto nível e os decompondo até o nível mais baixo, que é uma operação. De acordo com Barbosa et al. (2021), ao se basear na psicologia funcional, a HTA é capaz de relacionar os objetivos, motivações e consequências do que as pessoas fazem. Dessa forma, a HTA permite uma compreensão detalhada das atividades humanas, auxiliando na identificação de dificuldades e na proposição de melhorias tanto em sistemas quanto em procedimentos operacionais. Essa análise pode ser feita em forma de diagrama de hierarquia entre os objetivos ou em forma de tabela, ainda seguindo uma sequência, especificando problemas e recomendações para cada objetivo ou operação. 

## Metodologia
O modelo escolhido da HTA foi o de diagrama hierárquico, que de acordo com Barbosa et. al (2021) temos a respectiva legenda na figura 1 abaixo, também temos listadas na tabela 1 Na as tarefas analisadas e os respectivos integrantes do grupo que as realizaram.  

<font size="2"><p style="text-align: center">Figura 1: Legenda do diagrama.</p></font>

<center>

![legenda](../../assets/analiseHTA/legendaDiagramaHTA.jpeg)

</center>

<font size="2"><p style="text-align: center">Fonte: Barbosa et. al, 2021.</p></font>

<font size="2"><p style="text-align: center">Tabela 1: Análises realizadas.</p></font>

<center>

| Tarefa | Responsável |
| --- | --- |
| Calcular preços e prezos de entrega | Cláudio |
| Realizar compras na loja online | Elias |
| Emitir certificados digitais | Gabriel B. Bertolazi |
| Realizar pré-postagem | Gabriel F. J. Silva|
| Gerenciar minhas importações| Pablo |
| Rastrear encomendas | Ricardo |

</center>

<font size="2"><p style="text-align: center">Fonte: [Gabriel F. J. Silva](https://github.com/MMcLovin), 2024.</p></font>

## Análise das tarefas

### 1. Calcular preços e prazos de entrega
Abaixo, na Tabela 2, temos a representação da HTA em forma de tabela e na figura 2, a HTA em forma de diagrama para a tarefa de calcular preços e prazos pelo site dos Correios.

<font size="2"><p style="text-align: center">Tabela X: HTA em tabela para realizar uma pré-postagem.</p></font>

<center>

| objetivos / operações | problemas e recomendações |
| --- | --- |
| 0. Cálcular preços e prazos de entrega 1 > 2 | **input**: data da postagem, CEP, dados gerais do objeto e serviços opcionais <br>**plano**: preencher data da postagem, informar CEP de origem e destino, preencher dados do objeto e escolher serviços opcionais |
| 1. Informar Data da postagem |  |
| 2. Informar CEP de origem e destino 1 / 2 | **input**: CEP de origem e destino <br>**plano**: informar CEP de origem e destino e encontrar CEP (não sei o CEP) |
| 2.1 Informar CEP de origem e destino | |
| 2.2 Não sei o CEP 1 > 2 |**input**: Endereço de origem ou destino, e tipo do CEP <br>**plano**: Informar endereço e tipo do CEP, e encontrar o CEP <br> **feedback**: Abre um pop-up para encontrar o CEP com base no endereço  |
| 2.2.1 Informar endereço e tipo do CEP | |
| 2.2.2 Encontrar CEP | |
| 3. Informar dados do objeto 1 > 2| **plano**: Escolher tipo de serviço e informar formato do objeto <br>**feedback**: os campos variam conforme o tipo de escolha do usuário <br>**recomendação**: avisar o usuário que é necessário clicar em "adicionar" para registrar as informções inseridas nos campos|
| 1.2.2.1 Número e chave da NF-e | |
| 1.2.2.2 Informar descrição, quantidade e valor do objeto | |
| 1.2.2.3 Confirmar e adicionar informações | |
| 1.3 Escolher o tipo do serviço 1 / 2| **plano**: escolher entre o serviço SEDEX e PAC <br>**feedback**: o serviço escolhido é salvo e disponibilizado para vizualização e edição pelo usuário <br>**recomendação**: avisar o usuário caso um dos serviços não esteja disponível na região |
| 1.3.1 Escolher SEDEX | |
| 1.3.2 Escolher PAC | |
| 1.4 Adicionar pré-postagem ao carrinho | |
| 2 Gerenciar carrinho 1 / 2 / 3| **plano**: Prosseguir com a conclusão do pagamento ou inserir uma nova pré-postagem ou editar limpar os itens do carrinho <br>**feedback**: a tabela de itens no carrinho é atualizada de acordo com as ações do usuário <br>**problema**: não é possível apagar 1 item do carrinho quando há apenas 1 item <br>**recomendação**: identificar e mostrar o erro de não exclusão para o usuário |
| 2.1 Prosseguir com pagamento | |
| 2.2 Inserir nova pré-postagem | |
| 2.3 Limpar carrinho | |
| 3 Escolher a forma de pagamento 1 / 2 / 3|  **input**: dados do cartão de crédito <br>**feedback**: a página é atualizada conforme o meio de pagamento escolhido<br>**plano**: escolher netre pagar com cartão de crédito, boleto ou PIX <br>**recomendação**: caso não seja possivel selecionar uma opção em específico explicar para o usuário o motivo |
| 3.1 Pagar com cartão de crédito| |
| 3.2 Pagar com boleto| |
| 3.3 Pagar com PIX| |

</center>


<font size="2"><p style="text-align: center">Figura 2: .</p></font>

<font size="2"><p style="text-align: center">Fonte: [Claudio Henrique](https://github.com/claudiohsc), 2024.</p></font>

### 2. Realizar compras na loja online


<font size="2"><p style="text-align: center">Figura 3: .</p></font>

<font size="2"><p style="text-align: center">Fonte: [](https://github.com/), 2024.</p></font>

### 3. Emitir certificados digitais


<font size="2"><p style="text-align: center">Figura 4: .</p></font>

<font size="2"><p style="text-align: center">Fonte: [](https://github.com/), 2024.</p></font>


### 4. Realizar pré-postagem

Abaixo, na Tabela 5, temos a representação da HTA em forma de tabela e na figura 5, a HTA em forma de diagrama para a tarefa de realizar uma pré-postagem pelo site dos correios.

<font size="2"><p style="text-align: center">Tabela X: HTA em tabela para realizar uma pré-postagem.</p></font>

<center>

| objetivos | operações **problema**s e recomendações |
| --- | --- |
| 0 Realizar pré-postagem 1 > 2 > 3| **input**: dados da pré-postagem e meio de pagamento <br>**plano**: preencher dados da pré-postagem, gerenciar o carrinho e concluir a compra |
| 1 informar dados da pré-postagem 1 + 2| **input**: dados do remetente, destinatario e objeto <br>**plano**: informar dados do remetente e destinatário, informar dados do objeto, escolher o tipo de serviço e adicionar a pré-postagem ao carrinho <br>**recomendação**: informar ao usuário quais campos são obrigatórios |
| 1.1 informar destinatario e remetente | <br>**input**: Nome, Email, Telefone, CEP, Endereçõ e CPF <br>**feedback**: os dados inseridos são salvos e disponibilizados para edição pelo usuário <br>**plano**: informar nome, CEP e número do remetente e destinatário |
| 1.1.1 informar dados do remetente | |
| 1.1.2 informar dados do destinatario | |
| 1.2 informar dados do objeto 1 + 2 | **input**: formato e dimensões da embalagem e informações adiconais sobre o objeto <br>**plano**: selecionar o tipo da embalagem (carta, caixa ou cilindro) e as respectivas dimensões |
| 1.2.1 selecionar a embalagem do objeto e inserir dimensões | |
| 1.2.2 fornecer informações adicionais (1 / 2) > 3| **plano**: Informar dados da nota fiscal ou descrição do objeto, quantidade ou valor e clicar em inserir informações <br>**feedback**: os campos de dimensão variam conforme o tipo de embalagem escolhida e as informações adicionais são salvas em uma tabela ao final da página <br>**recomendação**: avisar o usuário que é necessário clicar em "adicionar" para registrar as informações inseridas nos campos|
| 1.2.2.1 Número e chave da NF-e | |
| 1.2.2.2 Informar descrição, quantidade e valor do objeto | |
| 1.2.2.3 Confirmar e adicionar informações | |
| 1.3 Escolher o tipo do serviço 1 / 2| **plano**: escolher entre o serviço SEDEX e PAC <br>**feedback**: o serviço escolhido é salvo e disponibilizado para vizualização e edição pelo usuário <br>**recomendação**: avisar o usuário caso um dos serviços não esteja disponível na região |
| 1.3.1 Escolher SEDEX | |
| 1.3.2 Escolher PAC | |
| 1.4 Adicionar pré-postagem ao carrinho | |
| 2 Gerenciar carrinho 1 / 2 / 3| **plano**: Prosseguir com a conclusão do pagamento ou inserir uma nova pré-postagem ou editar limpar os itens do carrinho <br>**feedback**: a tabela de itens no carrinho é atualizada de acordo com as ações do usuário <br>**problema**: não é possível apagar 1 item do carrinho quando há apenas 1 item <br>**recomendação**: identificar e mostrar o erro de não exclusão para o usuário |
| 2.1 Prosseguir com pagamento | |
| 2.2 Inserir nova pré-postagem | |
| 2.3 Limpar carrinho | |
| 3 Escolher a forma de pagamento 1 / 2 / 3|  **input**: dados do cartão de crédito <br>**feedback**: a página é atualizada conforme o meio de pagamento escolhido<br>**plano**: escolher netre pagar com cartão de crédito, boleto ou PIX <br>**recomendação**: caso não seja possivel selecionar uma opção em específico explicar para o usuário o motivo |
| 3.1 Pagar com cartão de crédito| |
| 3.2 Pagar com boleto| |
| 3.3 Pagar com PIX| |

</center>

<font size="2"><p style="text-align: center">Fonte: [Gabriel F. J. Silva](https://github.com/MMcLovin), 2024.</p></font>

<font size="2"><p style="text-align: center">Figura 5: HTA para realizar uma pré-postagem.</p></font>

<center>

![legenda](../../assets/analiseHTA/Pre-postagemHTA.jpg)

</center>

<font size="2"><p style="text-align: center">Fonte: [Gabriel F. J. Silva](https://github.com/MMcLovin), 2024.</p></font>

Para uma melhor vizualização, abra a imagem por [aqui](../../assets/analiseHTA/Pre-postagemHTA.jpg).

### 5. Gerenciar minhas importações


<font size="2"><p style="text-align: center">Figura 6: .</p></font>

<font size="2"><p style="text-align: center">Fonte: [](https://github.com/), 2024.</p></font>

### 6. Rastrear encomendas


<font size="2"><p style="text-align: center">Figura 7: .</p></font>

<font size="2"><p style="text-align: center">Fonte: [](https://github.com/), 2024.</p></font>


## Bibliografia

> - 


## Histórico de Versões

| Versão | Data | Descrição | Autor(es) | Revisor(es) |
| :----: | :--: | --------- | ----------- | ------ |
| `1.0`  | 05/05/2024 | Criação do documento | [Gabriel F. J. Silva](https://github.com/MMcLovin) |  |