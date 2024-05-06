# CMN-GOMS

## Introdução
A família GOMS (Goals, Operators, Methods, and Selection Rules) é uma abordagem amplamente reconhecida na área de IHC para analisar e prever o desempenho de usuários em sistemas computacionais, considerando que o usuário já sabe qual tarefa irá realizar. Esta família de modelos fornece uma estrutura sistemática para descrever as interações entre usuários e sistemas, abordando desde os objetivos que os usuários desejam alcançar até os métodos e operadores utilizados para alcançar esses objetivos, bem como as regras de seleção que guiam as escolhas dos usuários. 

A técnica escolhida da família GOMS foi a CMN-GOMS, que é caracterizada por uma estrutura hierárquica rigorosa, em que os objetivos são organizados de forma sequencial e os métodos (maneiras diferentes de se atingir um objetivo) são descritos de forma parecida com um pseudocódigo, incluindo submétodos e condicionais (Barbosa et. al, 2021). Essa técnica fornece uma visualização cuidadosa dos procedimentos realizados pelo usuário e das interações esperadas com o sistema, permitindo prever o desempenho e identificar possíveis problemas. Em suma, o CMN-GOMS é uma técnica robusta e informativa dentro da família GOMS, amplamente utilizada na análise e design de interfaces computacionais.

## Metodologia 
Cada integrante realizou a análise de tarefas das funcionalidades previamente designadas na última em [reunião de grupo](../../atas/ata3.md). Foram analisadas ao todo 6 tarefas, que podem ser vistas na Tabela 1, assim como os seus respectivos responsáveis.

<font size="2"><p style="text-align: center">Tabela 1: Tarefas analisadas realizadas.</p></font>

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

### 1. Calcular preços e prezos de entrega
Abaixo está a análise da funcionalidade de cálculo de preços e prazos de entrega, em formato de pseudocódigo, do site dos Correios.

```
GOAL 0: Calcular preços e prazos de entrega
    OP. 0.1: Abrir o site dos correios em um navegador web
    OP. 0.2: Ir até a opção “Preços e Prazos” na primeira seção do site

    GOAL 1: Informar Data da Postagem
        METHOD 1.A: Preencher Data da Postagem
        (SEL. RULE: O campo de data da postagem está visível na tela.)
        METHOD 1.A.A: Digitar a Data
        (SEL. RULE: O campo de data está vazio.)
            OP. 1.A.A.1: Clicar no campo de data.
            OP. 1.A.A.2: Digitar a data desejada.
            OP. 1.A.A.3: Confirmar a data digitada.

    GOAL 2: Informar CEP de Origem e Destino
        METHOD 2.A: Informar CEPs Utilizando Entrada de Texto
        (SEL. RULE: Os campos de CEP de origem e destino estão visíveis na tela.)
        METHOD 2.A.A: Preencher CEPs
        (SEL. RULE: Os campos de CEP estão vazios.)
            OP. 2.A.A.1: Clicar nos campos de CEP de origem e destino.
            OP. 2.A.A.2: Digitar os CEPs de origem e destino.
            OP. 2.A.A.3: Confirmar os CEPs digitados.
        METHOD 2.A.B: Não sei o CEP
        (SEL. RULE: o usuário não conhece o CEP de destino ou de origem)
            OP. 2.A.B.1: Clicar no campo "Não sei o CEP".
            OP. 2.A.B.2: Digitar um CEP ou um Endereço.
            OP. 2.A.B.3: Informar tipo do CEP.
            OP. 2.A.B.4: Clicar em "Buscar".
            OP. 2.A.B.5: verificar resultados de busca.
        
```

### 2. Realizar compras na loja online


### 3. Emitir certificados digitais


### 4. Realizar pré-postagem

Temos abaixo a análise, em formato de pseudocódigo, da tarefa em que um usuário realiza o cadastro e pagamento de uma pré postagem pelo site dos correios.

```
GOAL 0: Realizar uma pré-postagem nos Correios 
    OP. 0.1: Abrir o site dos correios em um navegador web
    OP. 0.2: Ir até a opção “pré-postagem” na seção de “Acesso Rápido”
    
    GOAL 1: Acessar a seção de pré postagem
        METHOD 1.A: Fazer login 
            (SEL. RULE: O usuário já possui uma conta)
            OP 0.1.A.1: Fornecer usuário e senha
            OP 0.1.A.2: efetuar login
        METHOD 0.B: Fazer cadastro 
            (SEL. RULE: O usuário ainda não possui uma conta)
            OP. 0.1.B.2: Fornecer dados pessoais
            OP. 0.1.B.2: Efetuar cadastro

    GOAL 2: Preencher os dados da pré-postagem 
        Goal 3: Preencher os dados do remetente
            OP 3: Clicar no botão "Remetente" para inserir os dados
            OP 3.1: Preencher os campos obrigatórios: Nome, CPF/CNPJ, Endereço, CEP, Telefone, Celular e E-mail
            OP 3.2: Opcionalmente, editar informações automáticas fornecidas pelo sistema
        
        Goal 4: Preencher os dados do destinatário
            OP 4.1: Clicar no botão "Destinatário" para inserir os dados
            OP 4.2: Preencher os campos obrigatórios: Nome, CPF/CNPJ, Endereço, CEP, Telefone, Celular e E-mail
        
        Goal 5: Preencher os dados do objeto
            OP 5.1: Selecionar o formato do objeto: envelope, caixa ou cilindro
            OP 5.2: Inserir peso e dimensões conforme solicitado
            OP 5.3: Opcionalmente, declarar o valor do produto
        
        Goal 6: Selecionar o serviço de entrega
            OP 6.1: Escolher o tipo de serviço: SEDEX, PAC, Mini Envios ou Carta
            OP 6.2: Se necessário, selecionar serviços adicionais associados ao serviço principal
        
        Goal 7: Adicionar dados complementares
            OP 7.1: Inserir informações adicionais, se aplicável, como NCM, RFID, Nota Fiscal ou Declaração de Conteúdo
            OP 7.2: Marcar a caixa de concordância com o termo de conhecimento
            OP 7.3: Marcar a declaração de que não será encaminhado objeto proibido

    GOAL 8: Gerenciar o carrinho de compras 
        METHOD 8.A: Prosseguir com o pagamento
        (SEL. RULE: A opção está clicável e o usuário não deseja fazer alterações)
            OP 8.A.1: Clicar no botão “Pagar” no canto esquerdo da tela
        
        METHOD 8.B: Limpar o carrinho
        (SEL. RULE: O Usuário quer tirar todos os itens do carrinho)
            OP 8.B.1: Clicar no botão “Limpar Carrinho” no canto esquerdo da tela
        
        METHOD 8.C: Inserir nova pré-postagem
        (SEL. RULE: O usuário deseja adicionar mais itens ao carrinho)
            OP 8.C.1: Criar uma nova pré-postagem
            OP 8.C.2: Prosseguir com pagamento
        
        METHOD 8.A: Selecionar e excluir pré-postagem
        (SEL. RULE: Há itens para serem selecionados e o usuário deseja editar o carrinho)
            OP 8.A.1: Selecionar pré-postagens na tabela de pré-postagens do carrinho
            OP 8.A.2: Excluir itens selecionados 
            OP 8.A.3: Prosseguir com pagamento

    GOAL 9: Realizar o pagamento 
        METHOD 9.A: Pagar com pix
        (SEL. RULE: A opção está clicável)
            OP 9.A.1: Selecionar a opção de pagamento com pix
            OP 9.A.2: Concluir o pagamento
        
        METHOD 9.B: Pagar com boleto
        (SEL. RULE: A opção está clicável)
            OP 9.B.1: Selecionar a opção de pagamento com boleto
            OP 9.B.2: Concluir o pagamento
        
        METHOD 9.C: Pagar com cartão de crédito
        (SEL. RULE: A opção está clicável)
            OP 9.C.1: Selecionar a opção de pagamento com cartão de crédito
            OP 9.C.2: Concluir o pagamento
```

### 5. Gerenciar minhas importações


### 6. Rastrear encomendas


## Referências

> 1. Barbosa, S. D. J.; Silva, B. S. da; Silveira, M. S.; Gasparini, I.; Darin, T.; Barbosa, G. D. J. (2021) Interação Humano-Computador e Experiência do usuário. Autopublicação. ISBN: 978-65-00-19677-1. Disponível em: <https://leanpub.com/ihc-ux>. Acesso em: 05 de Maio de 2024.

## Bibliografia

> 1. Alves, Douglas; Maciel, Geovanna. Análise de Tarefas. Repositório do Grupo Bilheteria Digital de Interação Humano Computador da Universidade de Brasília, 2023. Disponível em: <https://interacao-humano-computador.github.io/2023.1-BilheteriaDigital/analise-de-requisitos/analise-de-tarefas/goms/#bibliografia>. Acesso em: 05 de Maio 2023.
> 2. Barbosa, S. D. J.; Silva, B. S. da; Silveira, M. S.; Gasparini, I.; Darin, T.; Barbosa, G. D. J. (2021) Interação Humano-Computador e Experiência do usuário. Autopublicação. ISBN: 978-65-00-19677-1. Disponível em: <https://leanpub.com/ihc-ux>. Acesso em: 05 de Maio de 2024.


## Histórico de Versões

| Versão | Data | Descrição | Autor(es) | Revisor(es) |
| :----: | :--: | --------- | ----------- | ------ |
| `1.0`  | 05/05/2024 | Criação do documento | [Gabriel F. J. Silva](https://github.com/MMcLovin) |  |