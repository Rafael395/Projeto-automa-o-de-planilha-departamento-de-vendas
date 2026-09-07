# Projeto-automa-o-de-planilha-departamento-de-vendas
Um projeto pessoal baseado e uma planilha de vendas de uma empresa 

# Contexto
Neste projeto simularei o seguinte cenário: Uma empresa fictícia "J&J Soluções de Fornecimento" trabalha fazendo a ponte entre fornecedores e empresas, sendo uma empresa B2B, dentre seus fornecedores, 5 em especiais se destacam, sendo elas:
- Ferrero Metais: Uma empresa metalúrgica de pequeno porte que tem como foco produtos simples a base de metais;
- AHD Metais: Uma empresa metalúrgica de médio porte, seu foco são produtos com maior complexidade, por isso embora produzam alguns produtos que possam ser semelhantes a da Ferrero Metais, acabam tendo um custo médio maior e acabam não competindo direto por seus focos diferentes;
- Castor Madeira: Uma empresa de médio porte especializada em madeira vencendo peças brutas, tratadas e prensadas;
- Alto e Baixo: Plásticos & Borrachas: Uma empresa pequena focada em produtos derivados do petróleo, fazendo trabalho de purificação e refino de derivados do petróleo e vendendo o resultado a empresas que trabalhem com eles mas não queiram ter gastos investindo no refino e purificação dos mesmos;
- Santos Containers: Uma empresa focada na venda de containers, com o cargo chefe sendo barris de plásticos e metal, mas que está tentando entrar no mercado de paletes;

As 5 enviaram um relatório bruto com vendas, tendo enviado nomes do vendedor que fez a transação, a quantidade vendida e o item vendido, após os dados terem sido fundidos colocados juntos em uma planilha e devidamente separados por empresa, como na imagem a baixo:
<img width="1920" height="1020" alt="J J_DadosBrutos" src="https://github.com/user-attachments/assets/8cdca061-6896-4e40-b8eb-022b0203ad76" />

<img width="1920" height="1020" alt="J J_DadosBrutosFiltro" src="https://github.com/user-attachments/assets/c87a7bfe-e148-49ce-9609-7afae5c52b7e" />

Sendo assim, a J&J pediu que 3 coisas fossem realizadas.
1º - Os dados precisam ser tratados e transformados em planilhas, com a J&J fornecendo os dados necessários restantes como ID's de produtos e vendedores, e datas das vendas.

2º - A planilha precisa ser automatizada, para caso algum dado mude ou seja adicionado, a pesquisa baseada na mesma continue correta e precisa.

3º  - Uma dashboard em Power BI deve ser feita a partir da mesma junto de um relatório de vendas para melhor analise das relações de vendas, empresas e vendedores da empresa.

# Objetivos Resumidos
Tratamento de dados em planilha, criação de dashboard, automatização de planilha e criação de relatório de vendas

# O que foi feito

## 0º Etapa - Pós produção
Esta etapa foi adicionada após a finalização do documento em Excel, com o objetivo de dar duas informações, a primeira é que o arquivo tem uma senha de proteção, sendo a mesma "1234" que pode ser usada para desativar  proteção no mesmo, segundo, após baixar o arquivo, para que os macros funcionem, é necessário clicar com o botão direito nele, ir em propriedades, e então na aba de geral, ir em segurança e desbloquear para que os macros funcionem, caso não deseje rodar os macros, este processo é desnecessário.

## 1º Etapa - Tratamento de dados
### 1.1 - Primeiro tratamento
A primeira etapa envolveu a transformação dos dados, coletando os dados e fazendo a correlação com base no que foi fornecido, tendo sido isso os ID's dos itens, junto das datas das vendas, e a troca dos nomes das empresas por suas abreviações usadas dentro da J&J tendo sido este o resultado:
<img width="1920" height="1020" alt="J J_Dados_Pre_Tratamento" src="https://github.com/user-attachments/assets/96ac5056-9abf-4853-811e-1c1ccc7f95af" />

### 1.2 - Importação de dados essências
A segunda etapa envolve a importação de dados, sendo eles os dados dos vendedores e os dados das empresas, para assim ter acesso melhor a ID's, valores e datas relacionados a eles, com este tendo sido o resultado inicial:
<img width="1920" height="1020" alt="Funcionarios_Pre_Tratamento" src="https://github.com/user-attachments/assets/5b4d26b9-a325-47b8-a44d-2d6bd086f734" />
<img width="1920" height="1020" alt="FM_Pre_Tratamento" src="https://github.com/user-attachments/assets/68b7bda3-35d1-4b72-a0d2-7764577fe6d3" />
<img width="1920" height="1020" alt="CM_Pre_Tratamento" src="https://github.com/user-attachments/assets/f2e22966-6c81-4ff0-8b7b-b57a623d458b" />
<img width="1920" height="1020" alt="AB_Pre_Tratamento" src="https://github.com/user-attachments/assets/398478df-d20c-43ea-bc09-b6337a21e20e" />
<img width="1920" height="1020" alt="SC_Pre_Tratamento" src="https://github.com/user-attachments/assets/73c43092-f742-4aeb-9872-b3b8b8f3b387" />

### 1.3 - Tratamento inicial
Após os receber, um breve tratamento é necessário, transformando os dados em tabela, colocando as células com as devidas formatações e adicionando novas colunas úteis como margem de lucro e lucro bruto, com os seguintes resultados:
<img width="1920" height="1020" alt="FM_Tratado" src="https://github.com/user-attachments/assets/1349c55a-f4b8-42ab-bf1c-7063399a698e" />
<img width="1920" height="1020" alt="AHD_Tratado" src="https://github.com/user-attachments/assets/6a9ea060-9417-44ae-aa37-741d256ea3a2" />
<img width="1920" height="1020" alt="CM_Tratado" src="https://github.com/user-attachments/assets/c88b9daa-61a0-48c7-99b3-804a3151ad24" />
<img width="1920" height="1020" alt="AB_Tratado" src="https://github.com/user-attachments/assets/d1ed777c-eb7f-4c55-acc6-d7a2b1d19d4c" />
<img width="1920" height="1020" alt="SC_Tratado" src="https://github.com/user-attachments/assets/42875ceb-b7a9-4f89-862b-3162a705939f" />

E com isso, chegamos na planilha de vendedores, da qual adicionei novas medidas de analise para os vendedores e que está conectada a planilha de de vendas, mas irei apresentar por partes, começando com a planilhas de vendas, sendo ela:
<img width="1920" height="1020" alt="Vendedores_Tratado" src="https://github.com/user-attachments/assets/dd339af3-451e-42b6-b8de-903c8ecd8541" />

Podendo se analisar tanto o valor total vendido quanto a quantidade de vendas dos vendedores, além do numero de itens vendidos individualmente, é possível comparar com valores como datas de vendas e data de contratação para ter uma analise da performance de cada individuo.
E junto dela, é necessário se mostrar a planilha de vendas, totalmente refeita e atualizada
<img width="1920" height="1020" alt="Vendas_Tratado" src="https://github.com/user-attachments/assets/5b75810e-07ff-428c-9018-b4fc93b8caec" />

Com o uso de Procx acompanhado de cálculos para comissões, lucros brutos e margem de lucro bruto esta nova planilha se baseia nos ID's, quantidades compradas e datas para realizar os cálculos e coletas de informação, embora ela seria mais realista e eficiente com uma tabela dinâmica de preços que refletisse a inflação e alteração de preços, porém pela falta de informações para tornar isto possível no momento atual, este projeto em si trabalhará com preço único.
Outra tabela importante de se ter em mente, é a tabela auxiliar de valores agregados utilizados para simplificar o comando de procx na tabela de vendas, conforme a tabela de valores agregados junta as informações das planilhas especificas de cada empresa e alimenta a planilha de vendas com isso:
<img width="1920" height="1020" alt="Agregados" src="https://github.com/user-attachments/assets/7a7a95e0-b56a-4d5e-a69a-4f8872e83e50" />

### 1.4 - Menus
Após o tratamento inicial, foi feita a criação do menus, no qual colocarei 4 menus, dois de pesquisa e dois de adição com base em macros, primeiro, apresentarei os mais simples, os de pesquisa, baseados em procx, somase e cont.se, um tem como objetivo pesquisar quanto a um vendedor em especifico, enquanto o outro tem como objetivo pesquisar quanto a um produto em especifico, ambos baseados em ID para a pesquisa, com validação de dados certificando que a pesquisa esteja correta, com ambos em branco estando assim:
<img width="1920" height="1020" alt="Menus_vazio" src="https://github.com/user-attachments/assets/6bc92797-70f2-4c25-b09e-916253153e2a" />

E após a inserção dos devidos ID's, ficando da seguinte forma:
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/da60bc21-c1ff-4cc9-86f1-dcfaaf8ea57a" />

E por fim, quase finalizando o arquivo, chegamos na parte mais complexa dele, os menus para inserir um novo vendedor ou uma nova venda, feitos com macros em VBA do excel, ao se inserir os dados nos devidos menus, o macro irá os analisar, verificar se são condizentes com dedos pré estabelecidos na planilha, como ID's, depois irá verificar se eles são validos por si só, como datas de vendas que são anteriores a data de contratação de um vendedor, e por fim, após o fazer, ele adiciona os dados em suas devidas planilhas, seja a de vendas ou vendedores, ambos os menus em branco ficam desta maneira:
<img width="1920" height="1020" alt="Menus_vazios" src="https://github.com/user-attachments/assets/e07b3415-fd45-46d8-bfbf-40df9bca97b6" />

Agora irei adicionar um novo vendedor, com os seguintes dados:
<img width="1920" height="1020" alt="Novo_Vendedor" src="https://github.com/user-attachments/assets/c3448a46-3e30-44e2-8110-f2b4eb58f0aa" />
Após o adicionar aparece a seguinte mensagem:
<img width="1920" height="1020" alt="mensagem_vendedor_novo" src="https://github.com/user-attachments/assets/dbe74e50-4e7b-4a39-ad3a-435129a4273b" />

E a comparação do antes e depois com o novo vendedor adicionado, conforme nenhuma venda foi atribuída ao novo vendedor ainda, os valores dele apareceram como 0 ou nulos:
<img width="1920" height="1020" alt="Vendedores_Antes" src="https://github.com/user-attachments/assets/e52f9b73-d5cb-4dc1-bf3b-a02d47ca57aa" />
<img width="1920" height="1020" alt="Vendedores_Depois" src="https://github.com/user-attachments/assets/9483563c-30e8-4d74-adff-869e5d25a2f5" />

E agora, utilizando o novo ID e vendedor, iremos adicionar uma nova venda para Adriano:
<img width="1920" height="1020" alt="Nova_venda" src="https://github.com/user-attachments/assets/821e4c46-d6a1-45a9-8ac2-0428c570035a" />
<img width="1920" height="1020" alt="venda_registrada" src="https://github.com/user-attachments/assets/44c64d39-15e1-4603-8b1e-55b5dd5f4d0f" />

E agora o comparativo antes e depois da planilha de vendas:
<img width="1920" height="1020" alt="Vendas_Antes" src="https://github.com/user-attachments/assets/5bde36c5-a335-40f2-8ccd-fa358920c054" />
<img width="1920" height="1020" alt="Vendas_Depois" src="https://github.com/user-attachments/assets/dc499a2b-d2e2-4087-972c-9c574e1d8b8b" />

E por fim, a tabela de vendedores atualizada agora que Adriano tem uma venda:
<img width="1920" height="1020" alt="Vendedores_atualizada" src="https://github.com/user-attachments/assets/48f2ba40-4527-4f0b-a1b1-189056cc20b5" />

Por fim, antes de finalizar, vou apenas demonstrar alguns erros que poderiam ter sido feitos e como o macro iria lidar com eles:
1 - Adicionar venda com ID errado de vendedor:
<img width="1920" height="1020" alt="Erro_ID" src="https://github.com/user-attachments/assets/00e5303f-172f-4ba6-aba5-b6c721b5ec3d" />

2 - Adicionar venda com data de antes da contratação do vendedor 
<img width="1920" height="1020" alt="venda_antes_contratacao" src="https://github.com/user-attachments/assets/c2b01539-432b-45b7-958f-5a528235dfeb" />

3 - tentar adicionar campos em branco
<img width="1920" height="1020" alt="campo_branco" src="https://github.com/user-attachments/assets/2849241b-d0af-4ad2-b800-711e57e7655d" />

E por fim, este é o resultado final da planilha de Menus
<img width="1920" height="1020" alt="menus" src="https://github.com/user-attachments/assets/3bbda74a-cdc6-44e4-8ae6-d3a3e05adf6e" />


### 1.5 - Segurança
Finalizando a planilha, aplicando um processo de segurança simples do excel, travando a edição das células e formas, permitindo que apenas certas células possam ser editadas, com as de pesquisa tendo as de pesquisa de menu sem senha conforme a validação de dados já limita seu uso, e as demais, salvo as de adição de vendedores ou vendas que precisam de senha, tendo a edição proibida, assim deixando a planilha mais segura, com as seguintes prints do processo de forma resumida:
<img width="1920" height="1020" alt="seguranca" src="https://github.com/user-attachments/assets/119e9ec3-b71e-4d0a-a7a8-0adbe33663b2" />

<img width="1920" height="1020" alt="seguranca2" src="https://github.com/user-attachments/assets/e3c078ee-a72a-4524-ae7f-7f65f4e41c77" />

<img width="1920" height="1020" alt="seguranca3" src="https://github.com/user-attachments/assets/0ae06027-8ec6-4c28-8b89-b05e4e39589f" />

<img width="1920" height="1020" alt="seguranca4" src="https://github.com/user-attachments/assets/38f21829-a68d-4ed4-9213-29d7986c8732" />

<img width="1920" height="1020" alt="segurança5" src="https://github.com/user-attachments/assets/997b88a9-7f29-4f3c-a6f7-10f52b04d2b4" />

E assim finalizando o processo da criação e desenvolvimento da planilha.
