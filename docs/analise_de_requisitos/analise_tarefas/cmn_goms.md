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
| Calcular preços e prazos de entrega | Cláudio |
| Realizar compras na loja online | Elias |
| Emitir certificados digitais | Gabriel B. Bertolazi |
| Realizar pré-postagem | Gabriel F. J. Silva|
| Gerenciar minhas importações| Pablo |
| Rastrear encomendas | Ricardo |

</center>

<font size="2"><p style="text-align: center">Fonte: [Gabriel F. J. Silva](https://github.com/MMcLovin), 2024.</p></font>

## Análise das tarefas

### 1. Calcular preços e prazos de entrega
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

    GOAL 3: Informar Dados do Objeto
        METHOD 3.A: Escolher Tipo de Serviço e Formato do Objeto
        (SEL. RULE: Os menus de escolha de tipo de serviço e formato do objeto estão visíveis na tela.)
            METHOD 3.A.1: Selecionar Tipo de Serviço
            (SEL. RULE: O campo de seleção de tipo de serviço está vazio.)
                OP. 3.A.1.1: Clicar no campo de seleção de tipo de serviço.
                OP. 3.A.1.2: Escolher o tipo de serviço desejado.
            METHOD 3.A.2: Selecionar Formato do Objeto
            (SEL. RULE: O campo de seleção de formato do objeto está visível e não está marcado.)
                OP. 3.A.2.1: Marcar opção de formato de objeto.

            GOAL 4: Preencher informações de acordo com o formato
                METHOD 4.A: Escolher formato Caixa/Pacote.
                (SEL. RULE: A opção está vísivel e desmarcada)
                    METHOD 4.A.A: Escolher embalagem dos Correios
                    (SEL. RULE: o campo de seleção está visível e vazio)
                        OP. 4.A.A.1: Selecionar opção 'Embalagem dos Correios'
                        OP. 4.A.A.2: Selecionar Caixa de encomenda.
                        OP. 4.A.A.3: Preecher informação de peso em kilos.
                    METHOD 4.A.B: Escolher outra embalagem.
                    (SEL. RULE:  o campo de seleção está visível e vazio)
                        OP. 4.A.B.1: Selecionar opção 'Outra embalagem'.
                        OP. 4.A.B.2: Preecher informação de altura em centímetros.
                        OP. 4.A.B.3: Preecher informação de largura em centímetros.
                        OP. 4.A.B.4: Preecher informação de comprimento em centímetros.
                        OP. 4.A.B.5: Preecher informação de peso em kilos.
                METHOD 4.B: Escolher Formato Rolo/Cilindro ou Esfera.
                (SEL. RULE: a opção está visível e desmarcada)
                    OP. 4.B.1: Preecher informação de comprimento em centímetros.
                    OP. 4.B.2: Preecher informação de diâmetro em centímetros.
                    OP. 4.B.3: Preecher informação de peso em kilos.

    GOAL 5: Escolher Serviços Opcionais
        METHOD 5: Selecionar Serviços Opcionais
        (SEL. RULE: Os serviços opcionais estão listados na tela e estão desmarcados.)
            OP. 5.1: Clicar nas caixas de seleção dos serviços opcionais desejados.

    GOAL 6: Calcular Preços e Prazos
            OP. 6.1: Clicar no botão de 'Calcular'.
            OP. 6.2: Aguardar o resultado do cálculo.
```

### 2. Realizar compras na loja online


```
GOAL 0: Realizar Compra na loja online
    OP. 0.1: Abrir o site dos correios em um navegador web.
    OP. 0.2: selecionar a opção "Loja Online" localizada no menu suspenso comprar.

    GOAL 1: Buscar um produto
    METHOD 1.A: Encontre o produto.
        (SEL. RULE: O campo busca se apresenta vazio na tela)
        OP 1.A.1: Digite o nome do produto no campo Busca.
        OP 1.A.2: Clique no botão buscar.
        OP 1.A.3: Clique no produto encontrado.
    METHOD 1.A.A: Adicione filtros
        (SEL. RULE: O produto buscado é encontrado)
        OP 1.A.B.1: Filtre as buscas para encontrar o produto desejado
    METHOD 1.A.A.A: Receba notificação
        (SEL. RULE: O produto buscado não é encontrado)
        OP 1.A.B.C.1: Clique no botão "Clique aqui"
        OP 1.A.B.C.2: Insira um email e um prazo.
        OP 1.A.B.C.3: Clique em Confirmar.

        GOAL 2: Recalcular Valor dos produtos
                METHOD 2.A: Atualizar valor
                    (SEL. RULE: Há produtos no carrinho)
                    OP 2.A.1: Digite o um número no compo quantidade do produto desejado.
                    OP 2.A.1: Clique em Recalcular para atualizar.

            GOAL 3: Cálculo do frete
                METHOD 3.A: Informar CEP.
                    (SEL. RULE: o campo para inserir o CEP se encontra vazio)
                    OP 3.A.1: Selecione o páis e insira o CEP de destino válido.
                    OP 3.A.2: Clique em Calcular.
                    OP 3.A.3: Clique em Fechar Pedido.
                METHOD 3.A.A: Informar CEP.
                    (SEL. RULE: o usuário desconhece o CEP)
                    OP 3.A.B.1: Clique na opção "Busca CEP".
                    OP 3.A.B.3: Digite um endereço ou cep.
                    OP 3.A.B.3: Veja os resutados.
                    OP 3.A.B.4: Insira o CEP no campo Cálculo e clique em calcular.
                    OP 3.A.B.5: Clique em Fechar Pedido.

            
                GOAL 4: Identificação
                    METHOD 4.A: Login
                        (SEL. RULE: O usuário não se encontra logado)
                        OP 4.A.1: Faça o Login.
                        OP 4.A.2: Clique em loja Correios online.
                        OP 4.A.3: Clique em ao Carrinho.
                        OP 4.A.4: Clique em fechar pedido.
                    METHOD 4.B: Cadastro
                        (SEL. RULE: O usuário não possui cadastro)
                        OP 4.A.B.1: Faça o Cadastro.
                        OP 4.A.B.1: Faça o Login.
                        OP 4.A.B.2: Clique em loja Correios online.
                        OP 4.A.B.3: Clique em ao Carrinho.
                        OP 4.A.B.4: Clique em fechar pedido.

                    
                    GOAL 5: Fechando Pedido
                        METHOD 5.A: Finalizar Compra
                            OP 5.A.1: Verifique o endereço de entrega.
                            OP 5.A.2: Verifique a forma de entrega.
                            OP 5.A.3: Verifique a forma de pagamento.
                            OP 5.A.4: Clique em Finalizar Compra.
```

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
        GOAL 3: Preencher os dados do remetente
            OP 3: Clicar no botão "Remetente" para inserir os dados
            OP 3.1: Preencher os campos obrigatórios: Nome, CPF/CNPJ, Endereço, CEP, Telefone, Celular e E-mail
            OP 3.2: Opcionalmente, editar informações automáticas fornecidas pelo sistema
        
        GOAL 4: Preencher os dados do destinatário
            OP 4.1: Clicar no botão "Destinatário" para inserir os dados
            OP 4.2: Preencher os campos obrigatórios: Nome, CPF/CNPJ, Endereço, CEP, Telefone, Celular e E-mail
        
        GOAL 5: Preencher os dados do objeto
            OP 5.1: Selecionar o formato do objeto: envelope, caixa ou cilindro
            OP 5.2: Inserir peso e dimensões conforme solicitado
            OP 5.3: Opcionalmente, declarar o valor do produto
        
        GOAL 6: Selecionar o serviço de entrega
            OP 6.1: Escolher o tipo de serviço: SEDEX, PAC, Mini Envios ou Carta
            OP 6.2: Se necessário, selecionar serviços adicionais associados ao serviço principal
        
        GOAL 7: Adicionar dados complementares
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
        
        METHOD 8.D: Selecionar e excluir pré-postagem
        (SEL. RULE: Há itens para serem selecionados e o usuário deseja editar o carrinho)
            OP 8.D.1: Selecionar pré-postagens na tabela de pré-postagens do carrinho
            OP 8.D.2: Excluir itens selecionados 
            OP 8.D.3: Prosseguir com pagamento

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

Abaixo está a análise da funcionalidade minhas importações, em formato de pseudocódigo, do site dos Correios.

```
GOAL 0: Gerenciar minhas importações 
    OP. 0.1: Abrir o site dos correios em um navegador web
    GOAL 1: Acessar “Meu Correios“
        OP. 1.1: Deslocar cursor do mouse para  Faça Login ou Cadastre-se 
        OP. 1.2: Deslocar cursor do mouse para  Meu Correios 
        OP. 1.3: Clicar com o botão esquerdo do mouse
        METHOD 1.A: Fazer login 
        (SEL. RULE: O usuário já possui uma conta)
            OP. 1.A.1: Fornecer usuário e senha
            OP. 1.A.2: Efetuar login
        METHOD 1.B: Fazer cadastro 
        (SEL. RULE: O usuário ainda não possui uma conta)
            OP. 1.B.1: Fornecer dados pessoais
            OP. 1.B.2: Efetuar cadastro
            OP. 1.B.3: Confirmar cadastro
            OP. 1.B.4: voltar a method 1.a
        METHOD 1.C: Esqueci minha senha
        (SEL. RULE: O usuário possui uma conta, porém não recorda da autenticação)
            OP. 1.C.1: Selecionar meio de recuperação
            OP. 1.C.2: Selecionar tipo de usuário
            OP. 1.C.3: Informar nº do documento ou idCorreios
            OP. 1.C.4: Clicar em prosegruir
            OP. 1.C.5: Confirmar código recebido
            OP. 1.C.6: Inserir nova senha
            OP. 1.C.7: Confirmar
            OP. 1.C.8: voltar a method 1.a
    GOAL 2: Acessar “Minhas Importações“
        OP. 2.1: Rola o scroll do mouse ate Acesso rápido
        OP. 2.2: Deslocar cursor do mouse para  Minhas Importações
        OP. 2.3: Clicar com o botão esquerdo do mouse
        OP. 2.4: Deslocar cursor do mouse para  Entendi na caixa de noticia importante
        OP. 2.5: Clicar com o botão esquerdo do mouse
    GOAL 3: Busca importação
        METHOD 3.A: Registro de importação no sistema
        (SEL. RULE: Importação já listada)
            OP. 3.A.1: Deslocar cursor do mouse para ícone detalhar
            OP. 3.A.2: Clicar com o botão esquerdo do mouse
            OP. 3.A.3: Ler situação alfandegaria
        METHOD 3.B: Registro de importação ausente
        (SEL. RULE: Importação não listada na tabela)
            OP. 3.B.1: Deslocar cursor do mouse para input Pesquisar Encomenda
            OP. 3.B.2: Clicar com o botão esquerdo do mouse
            OP. 3.B.3: Inserir código da encomenda
            OP. 3.B.4: Deslocar cursor do mouse para botão pesquisar
            OP. 3.B.5: Clicar com o botão esquerdo do mouse
            OP. 3.B.6: voltar a method 3.a
    GOAL 4: Emitir boleto
        OP. 4.1: Deslocar cursor do mouse para ícone Visualizar DIS
        OP. 4.2: Clicar com o botão esquerdo do mouse

```

### 6. Rastrear encomendas

```
GOAL 0: Rastrear uma encomenda.
    OP. 0.1: Abrir o site doscorreios em um navegador web.
    OP. 0.2: Ir para a seção "Acompanhe seu Objeto" no começo do site.

    GOAL 1: Informar o código de rastreamento.
        METHOD 1.A: Informar o código de rastreamento no campo abaixo de "Acompanhe seu Objeto".
        (SEL. RULE: Rastreamento de encomendas nacionais)
            OP. 1.A.1: Escrever o código de rastreamento.
            OP. 1.A.2: Clicar na lupa ao lado do campo preenchido.

        METHOD 1.B: Informar o código de rastreamento na tela de rastreamento.
        (SEL. RULE: Rastreamento de encomendas em outros países)
            OP. 1.B.1: Clicar na lupa embaixo do campo "Acompanhe seu Objeto".
            OP. 1.B.2: Clicar em "Rastreamento em outros países" nos 3 traços do lado esquerdo da tela.
            OP. 1.B.3: Digitar o código de rastreamento internacional no campo "Enter tracking number".

    GOAL 2: Informar a captcha contida na imagem.
        METHOD 2.A: Digitar o texto contido na imagem.
        (SEL. RULE: Imagem possuir texto leǵivel para poder ser escrito)
            OP. 2.A.1: Escrever com o teclado a captcha contida na imagem.

        METHOD 2.B: Selecionar outra imagem.
        (SEL. RULE: Texto da imagem não possui letras legíveis)
            OP. 2.B.1: Clicar em recarregar imagem.
            OP. 2.B.2: Caso o texto esteja legível, ir ao method 2.A, caso contrário, ir ao method 2.B.

    GOALS 3: Verificar informações do objeto
        METHOD 3.A: Ir até a consulta
        (SEL. RULE: Os dados de código de rastreamento e captcha na imagem foram inseridos corretamente)
            OP. 3.A.1: Clicar com o botão esquerdo do mouse no botão "Consultar".
```

<font size="2"><p style="text-align: center">Fonte: [Ricardo Augusto](https://github.com/avmricardo), 2024.</p></font>

## Referências

> 1. Barbosa, S. D. J.; Silva, B. S. da; Silveira, M. S.; Gasparini, I.; Darin, T.; Barbosa, G. D. J. (2021) Interação Humano-Computador e Experiência do usuário. Autopublicação. ISBN: 978-65-00-19677-1. 

## Bibliografia

> 1. Alves, Douglas; Maciel, Geovanna. Análise de Tarefas. Repositório do Grupo Bilheteria Digital de Interação Humano Computador da Universidade de Brasília, 2023. Disponível em: <https://interacao-humano-computador.github.io/2023.1-BilheteriaDigital/analise-de-requisitos/analise-de-tarefas/goms/#bibliografia>. Acesso em: 05 de Maio 2023.
> 2. Barbosa, S. D. J.; Silva, B. S. da; Silveira, M. S.; Gasparini, I.; Darin, T.; Barbosa, G. D. J. (2021) Interação Humano-Computador e Experiência do usuário. Autopublicação. ISBN: 978-65-00-19677-1.

## Histórico de Versões

| Versão | Data | Descrição | Autor(es) | Revisor(es) |
| :----: | :--: | --------- | ----------- | ------ |
| `1.0`  | 05/05/2024 | Criação do documento | [Gabriel F. J. Silva](https://github.com/MMcLovin) |  |
| `1.1`  | 05/05/2024 | Adiciona GOMS realizar pré-postagem | [Gabriel F. J. Silva](https://github.com/MMcLovin) |  |
| `1.2`  | 05/05/2024 | Adiciona GOMS calcular preços e prazos de entrega| [Claudio Henrique](https://github.com/claudiohsc) |  |
| `1.3`  | 06/05/2024 | Adiciona GOMS realizar compras na loja online | [Elias F. Oliveira](https://github.com/EliasOliver21) |  |
| `1.4`  | 06/05/2024 | Adiciona GOMS gerenciar minhas importações | [Pablo S. Costa](https://github.com/pabloheika) |  |
