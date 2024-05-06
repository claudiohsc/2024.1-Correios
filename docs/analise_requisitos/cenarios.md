# Cénarios
    
## Introdução
Os cenários na Interação Humano-Computador são essencialmente histórias que descrevem pessoas realizando uma atividade específica relacionada ao uso de uma aplicação. Eles são uma ferramenta poderosa no processo de design de IHC, pois requerem muito menos recursos que outras ferramentas como, por exemplo, modelos e protótipos complexos. Cada cenário descreve um caminho possível em um caso de uso, narrando as ações dos usuários, eventos que ocorrem e mudanças no ambiente, como podemos ver na descrição das características de um cenário na tabela 1. Ao serem utilizados em conjunto com personas, os atores dos cenários são as próprias personas, o que facilita a compreensão das necessidades e motivações dos usuários. 

É importante ressaltar que não é necessário criar cenários para todas as tarefas e situações possíveis, mas sim focar inicialmente nas tarefas principais e abordar as tarefas secundárias conforme o tempo permitir
 <a id="anchor_1" href="#REF1"> <sup>1</sup> </a>.

<font size="2"><p style="text-align: center">Tabela 1 - Características de um cenário </p></font> 

| Característica | Descrição|
| -------------- | ---------|
| ambiente ou contexto | detalhes da situação que motivam ou explicam os objetivos, ações e reações dos atores do cenário |
| atores | pessoas interagindo com o computador ou outros elementos do ambiente; características pessoais relevantes ao cenário |
| objetivos | efeitos na situação que motivam as ações realizadas pelos atores |
| planejamento | atividade mental dirigida para transformar um objetivo em um comportamento ou conjunto de ações |
| ações | comportamento observável |
| eventos | ações externas ou reações produzidas pelo computador ou outras características do ambiente, algumas delas podem ser ocultas ao ator mas importantes para o cenário |
| avaliação | atividade mental dirigida para interpretar a situação |

<font size="2"><p style="text-align: center">Fonte: Barbosa et al. (2021). Interação Humano-Computador e Experiência do usuário. Autopublicação. ISBN: 978-65-00-19677-1. Disponível em: https://leanpub.com/ihc-ux. Acesso em: 21 de Abril de 2024.</p></font> 

## Cenários realizados

Na tabela 2 está descrito qual funcionalidade cada integrante ficou resposnável para realizar os cenários presentes neste artefato.

<font size="2"><p style="text-align: center">Tabela 2: Análises realizadas.</p></font>

<center>

| Tarefa | Responsável |
| --- | --- |
| Calcular preços e prazos de entrega | Cláudio |
| Emitir certificados digitais | Gabriel B. Bertolazi |
| Realizar pré-postagem | Gabriel F. J. Silva|
| Realizar compras na loja online | Elias |
| Gerenciar minhas importações| Pablo |
| Rastrear encomendas | Ricardo |

</center>

<font size="2"><p style="text-align: center">Fonte: [Ricardo Augusto](https://github.com/avmricardo), 2024.</p></font>

### Cálculo de preços e prazos de entrega

Atores: [Gabriel Anacleto Saraiva](https://interacao-humano-computador.github.io/2024.1-Correios/analise_de_requisitos/personas/)


Gabriel Anacleto Saraiva, um comerciante de 20 anos, logo pela manhã vai para a empresa de camisetas e canecas personalizadas e já separa as encomendas que devem ser enviadas ainda no horário limite daquele dia. Ele recebeu um total de 5 pedidos durante o período que estava fora do seu posto de trabalho, dessa forma ele precisa ter uma previsão de quanto irá pagar para realizar o envio dos seus produtos. Nessa parte da manhã ele organiza e atualiza o estoque de todos os produtos, e logo em seguida entra no site do Correios para realizar o cálculo de preços e do prazo de entrega, e assim informar aos seus clientes.

Assim que o Gabriel entra no site, ele logo clica na opção de "Preços e Prazos" onde visualiza uma nova página para começar o preenchimento das informações do objeto. Como ele deseja enviar no mesmo dia, precisa ser rápido para calcular e enviar os produtos na parte da tarde, dessa forma já inicia colocando a data do mesmo dia e preenchendo com o CEP do seu endereço. Após isso, ele verifica o CEP informado pelo cliente e preenche no site na parte "CEP de destino". Como os seus produtos são camisetas e não ocupam muito espaço, o Gabriel escolhe o tipo de serviço "PAC" e o formato de de "Caixa/pacote". Seguindo os passos do site, ele agora escolhe a opção de "Outra embalagem" e preeche com as dimensões da sua própria caixa de envio: altura, largura, comprimento e o peso.

Ao terminar de preencher todas as informações do objeto, Gabriel não necessita de Serviços opcionais e então clica no botão "Calcular", o que o leva a outra página do Correios com os valores estimados que Gabriel pagará na hora de enviar o seu produto. Satisfeito com os resultados, Gabriel informa o valor e as informações ao seu cliente e segue para a simulação do seu próximo produto.

### Realização de Pré-postagem

Atores: [José Ricardo](https://interacao-humano-computador.github.io/2024.1-Correios/analise_de_requisitos/personas/) (Cliente dos Correios)

José Ricardo Gomes, influenciador digital, recebe um produto para sua nova campanha publicitária, porém, descobre que o produto está danificado de tal forma que impede o seu uso, impossibilitando a divulgação de sua experiência em suas redes. José entra em contato com a marca, que se prontificou a mandar um novo produto, mas pede que, caso seja possível, José retorne o produto danificado para que eles possam examiná-lo.
José lembra que há uma agência dos correios perto de sua casa e, com pressa, opta por realizar a pré-postagem pelo site para evitar filas. Ao acessar a seção de pré-postagem e fazer o login, ele preenche os dados do remetente e destinatário, garantindo que as informações obrigatórias estejam corretas. Em seguida, ele insere os detalhes do objeto, como formato, peso e dimensões, além de declarar o valor do produto. Como parte das informações complementares, José decide informar a NF-e, fornecendo o respectivo número e chave.

Em seguida José marca a caixa de checagem do termo de conhecimento ao final da página, satisfeito com todas as informações inseridas, ele adiciona o objeto ao carrinho de compras. Ao revisar o carrinho, José confirma que todas as informações estão corretas e prossegue para realizar o pagamento. EntrE as opções disponíveis, ele opta por pagar com cartão de crédito e completa o processo, se preparando para ir à agência dos correios.

### Loja dos Correios

Atores: [Erivaldo Virginio Silva](https://interacao-humano-computador.github.io/2024.1-Correios/analise_de_requisitos/personas/)

Erivaldo Virginio Silva, com 30 anos é um advogado habilidoso e muito capacitado que tabalha em um escritório de advocacia juntamente com outros advogados seus colegas. Na sua rotina diária o mesmo necessita de utilizar envelopes e papéis que ele adquiri dos correios, em uma certa manhã comum de trabalho Erivaldo precisa de alguns envelopes e decide dar uma rápida passada em uma agência dos correios mais próxima, mas quando chega lá descobre que o estoque de envelopes da agência esta vazio em e não há previsão de chegada em menos de 20 dias úteis, então o mesmo decide entrar na loja online dos correios para adquirir alguns e chegarem via sedex ao escritório.
Quando Erivaldo entra no site dos correios ele entra nas opções de compra e navega até a loja online dos correios, o mesmo então faz uma busca e encontra o que precisa seleciona a quantidade e adiciona ao carrinho, logo após realiza o seu cadastro para adicionar suas informações pessoas como endereço e cpf dentre outros, Erivaldo então segue para a etapa de pagamento seleciona a opção de compra com cartão de crédito para uma maior agilidade do processo e sua compra então é finalizada rapidamente,após finalizar a compra Erivaldo ve que os envelopes chegarão ao escritório em 3 dias úteis resolvendo seu problema, pois não poderia esperar 20 dias.

Erivaldo ao conclui ao final de tudo que o serviço da loja online o auxiliou, mas o mesmo não ficou muito satisfeito quanto a usabilidade e visual da página, pois a mesma tem um estilo ultrapassado, itens mal dispostos, recursos que não funcioman, redirecionamentos desnecessários, falta liberdade para o usuário nas etapas de finalização de compra. Devido a experiência que Erivaldo obteve com o site da loja o mesmo se ve totalmente contrário ao pensamento de voltar a utilizar o site.

### Minhas importações

Atores: [Gabriel Anacleto Saraiva](https://interacao-humano-computador.github.io/2024.1-Correios/analise_de_requisitos/personas/)

Gabriel Anacleto Saraiva, um comerciante de 20 anos, enfrentou um contratempo quando uma peça de sua valiosa máquina de sublimação quebrou. Dada a complexidade e o custo do equipamento, ele empreendeu uma busca detalhada pela peça de reposição, resultando na necessidade de importá-la. Durante os dias seguintes, Gabriel monitorou incessantemente o site dos Correios, ansioso pela chegada da peça, já que a ausência de um sistema de notificação dos Correios o deixava no escuro sobre possíveis problemas com a entrega.

Para verificar o status da encomenda, Gabriel navegava até o site dos Correios, fazia login em "Meu Correios" e selecionava "Minhas Importações", onde inseria o código de rastreamento, pois nem sempre é incluso de forma automática pelo documento cadastrado. Esse acompanhamento era essencial, pois qualquer contratempo poderia atrasar ou até impedir a entrega, acarretando mais prejuízos. Em caso de problemas, ele tinha um prazo de quinze dias para resolvê-los antes que o pacote fosse retornado ao remetente. Nesta ocasião, sua encomenda foi inspecionada pela alfândega e taxada pela entrega e pela Receita Federal. Gabriel gerou um boleto no site dos Correios e, após a confirmação do pagamento, seu pedido foi liberado e finalmente entregue.

Embora Gabriel tenha resolvido a questão, ele achou o processo exaustivo e burocrático, deixando-o insatisfeito com a solução oferecida pelos Correios.

### Rastreamento de encomendas

Atores: [João Victor Ribeiro](https://interacao-humano-computador.github.io/2024.1-Correios/analise_de_requisitos/personas/)

João Victor Ribeiro, um porteiro de 55 anos, chega em casa após um longo dia de trabalho. Depois de tomar um banho e jantar, ele se prepara para relaxar um pouco antes de ir dormir. Enquanto assiste TV, ele se lembra de que fez algumas compras online recentemente e decide verificar o status de suas encomendas nos Correios, já que ele espera ansiosamente por algumas ferramentas e artigos para casa que comprou para melhorar suas tarefas diárias.

Ele pega seu notebook e pede ao seu filho para ajudá-lo a rastrear as encomendas. Seu filho, familiarizado com o procedimento, acessa o site dos Correios e, junto com João, entra na seção de rastreamento de encomendas.

João observa enquanto seu filho insere os códigos de rastreamento das encomendas que ele fez. O site dos Correios exibe então o status de cada pacote. João fica aliviado ao ver que a maioria das suas encomendas está a caminho e deve chegar em breve. No entanto, uma das encomendas apresenta um status de "Objeto não encontrado", o que deixa João um pouco preocupado. Ele decide clicar no código de rastreamento para obter mais detalhes e descobrir o motivo pelo qual a encomenda não está sendo localizada. Após analisar as informações adicionais, João percebe que a encomenda ainda não foi postada pelo vendedor e, portanto, não há informações disponíveis sobre o seu trajeto.

## Referências Bibliográficas
> <a id="REF1" href="#anchor_1">1.</a> Barbosa, S. D. J.; Silva, B. S. da; Silveira, M. S.; Gasparini, I.; Darin, T.; Barbosa, G. D. J. (2021) Interação Humano-Computador e Experiência do usuário. Autopublicação. ISBN: 978-65-00-19677-1.

## Bibliografia

> 1. CORREIOS. Correios. Disponível em: <https://www.correios.com.br/>. Acesso em: 21 de Abril de 2024.
> 2. Barbosa, S. D. J.; Silva, B. S. da; Silveira, M. S.; Gasparini, I.; Darin, T.; Barbosa, G. D. J. (2021) Interação Humano-Computador e Experiência do usuário. Autopublicação. ISBN: 978-65-00-19677-1. 

## Histórico de versão

| Versão | Data | Descrição | Autor(es) | Revisor(es) |
|:-:|:-:|:-:|:-:|:-:|
|`1.0`| 21/04/2024 | Criação do documento e cenário de pré-postagem | [Gabriel F. J. Silva](https://www.github.com/MMcLovin) | [Pablo S. Costa](https://www.github.com/pabloheika) |
