# CMN-GOMS

## Introdução

## Metodologia 

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


### 2. Realizar compras na loja online


### 3. Emitir certificados digitais


### 4. Realizar pré-postagem

    Temos abaixo a análise em formato de pseudocódigo da tarefa em que um usuário realiza o cadastro e pagamento de uma pré postagem pelo site dos correios
```
GOAL 0: Realizar uma pré-postagem nos Correios 
    OP. 0.1: Abrir o site dos correios em um navegador web
    OP. 0.2: Ir até a opção “pré-postagem” na seção de “Acesso Rápido”
    
    GOAL 1: Acessar a seção de pré postagem
        METHOD 1.A: Fazer login 
            OP 0.1.A.1: Fornecer usuário e senha
            OP 0.1.A.2: efetuar login
        METHOD 0.B: Fazer cadastro 
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
            OP 8.A.1: Clicar no botão “Pagar” no canto esquerdo da tela
        
        METHOD 8.B: Limpar o carrinho
            OP 8.B.1: Clicar no botão “Limpar Carrinho” no canto esquerdo da tela
        
        METHOD 8.C: Inserir nova pré-postagem
            OP 8.C.1: Criar uma nova pré-postagem
            OP 8.C.2: Prosseguir com pagamento
        
        METHOD 8.A: Selecionar e excluir pré-postagem
            OP 8.A.1: Selecionar pré-postagens na tabela de pré-postagens do carrinho
            OP 8.A.2: Excluir itens selecionados 
            OP 8.A.3: Prosseguir com pagamento

    GOAL 9: Realizar o pagamento 
        METHOD 9.A: Pagar com pix
            OP 9.A.1: Selecionar a opção de pagamento com pix
            OP 9.A.2: Concluir o pagamento
        
        METHOD 9.B: Pagar com boleto
            OP 9.B.1: Selecionar a opção de pagamento com boleto
            OP 9.B.2: Concluir o pagamento
        
        METHOD 9.C: Pagar com cartão de crédito
            OP 9.C.1: Selecionar a opção de pagamento com cartão de crédito
            OP 9.C.2: Concluir o pagamento
```

### 5. Gerenciar minhas importações


### 6. Rastrear encomendas


## Bibliografia

> 1. Alves, Douglas; Maciel, Geovanna. Análise de Tarefas. Repositório do Grupo Bilheteria Digital de Interação Humano Computador da Universidade de Brasília, 2023. Disponível em: <https://interacao-humano-computador.github.io/2023.1-BilheteriaDigital/analise-de-requisitos/analise-de-tarefas/goms/#bibliografia>. Acesso em: 05 de abril 2023.
> 2. Barbosa, S. D. J.; Silva, B. S. da; Silveira, M. S.; Gasparini, I.; Darin, T.; Barbosa, G. D. J. (2021) Interação Humano-Computador e Experiência do usuário. Autopublicação. ISBN: 978-65-00-19677-1. Disponível em: <https://leanpub.com/ihc-ux>. Acesso em:  13 de Abril de 2024.


## Histórico de Versões

| Versão | Data | Descrição | Autor(es) | Revisor(es) |
| :----: | :--: | --------- | ----------- | ------ |
| `1.0`  | 05/05/2024 | Criação do documento | [Gabriel F. J. Silva](https://github.com/MMcLovin) |  |