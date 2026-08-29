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
## 1º Etapa - Tratamento de dados
### 1.1 - Primeiro tratamento
A primeira etapa envolveu a transformação dos dados, coletando os dados e fazendo a correlação com base no que foi fornecido, tendo sido isso os ID's dos itens, junto das datas das vendas, e a troca dos nomes das empresas por suas abreviações usadas dentro da J&J tendo sido este o resultado:
<img width="1920" height="1020" alt="J J_Dados_Pre_Tratamento" src="https://github.com/user-attachments/assets/96ac5056-9abf-4853-811e-1c1ccc7f95af" />

### 1.2 - Importação de dados essências
A segunda etapa envolve a importação de dados, sendo eles os dados dos vendedores e os dados das empresas, para assim ter acesso melhor a ID's, valores e datas relacionados a eles, com este tendo sido o resultado inicial:
<img width="1920" height="1020" alt="Funcionarios_Pre_Tratamento" src="https://github.com/user-attachments/assets/5b4d26b9-a325-47b8-a44d-2d6bd086f734" />
<img width="1920" height="1020" alt="FM_Pre_Tratamento" src="https://github.com/user-attachments/assets/68b7bda3-35d1-4b72-a0d2-7764577fe6d3" />
<img width="1920" height="1020" alt="AHD_Pre_Tratamento" src="https://github.com/user-attachments/assets/7f7b2085-8639-4721-b4a9-b207734f4f51" />
<img width="1920" height="1020" alt="CM_Pre_Tratamento" src="https://github.com/user-attachments/assets/f2e22966-6c81-4ff0-8b7b-b57a623d458b" />
<img width="1920" height="1020" alt="AB_Pre_Tratamento" src="https://github.com/user-attachments/assets/398478df-d20c-43ea-bc09-b6337a21e20e" />
<img width="1920" height="1020" alt="SC_Pre_Tratamento" src="https://github.com/user-attachments/assets/73c43092-f742-4aeb-9872-b3b8b8f3b387" />

### 1.3 - Tratamento inicial
Após os receber, um breve tratamento é necessário, transformando os dados em tabela, colocando as células com as devidas formatações e adicionando novas colunas úteis como margem de lucro e lucro bruto, com os seguintes resultados:
<img width="1920" height="1020" alt="FM_Tratado" src="https://github.com/user-attachments/assets/1349c55a-f4b8-42ab-bf1c-7063399a698e" />
<img width="1920" height="1020" alt="AHD_Tratado" src="https://github.com/user-attachments/assets/09b559f1-eea9-4150-96e5-dead193e2cb4" />
<img width="1920" height="1020" alt="CM_Tratado" src="https://github.com/user-attachments/assets/c88b9daa-61a0-48c7-99b3-804a3151ad24" />
<img width="1920" height="1020" alt="AB_Tratado" src="https://github.com/user-attachments/assets/d1ed777c-eb7f-4c55-acc6-d7a2b1d19d4c" />
<img width="1920" height="1020" alt="SC_Tratado" src="https://github.com/user-attachments/assets/42875ceb-b7a9-4f89-862b-3162a705939f" />
