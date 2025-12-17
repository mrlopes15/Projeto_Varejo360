Varejo 360 — Monitoramento Inteligente de Ocorrências no Varejo
Este projeto simula um cenário real de varejo, com foco em identificar problemas operacionais a partir de reclamações de clientes, transformar esses dados em alertas acionáveis e apoiar a tomada de decisão gerencial.
A proposta não é apenas analisar dados, mas mostrar como dados, automação e visualização podem trabalhar juntos para gerar valor real para o negócio.
1 - Contexto do problema
É muito comum o cliente reclamar que um produto “consta em estoque, mas não está disponível na loja”. Esse tipo de situação gera insatisfação, perda de venda e desgaste da marca.
O desafio abordado neste projeto foi responder perguntas como:
– Onde estão concentradas as ocorrências negativas?
– Qual o peso da ruptura virtual na insatisfação do cliente?
– Quais produtos exigem ação operacional imediata?
– Esse problema está recorrente ao longo do tempo?
– Como priorizar ações por loja e por produto?

2 - Solução proposta
Foi construída uma solução ponta a ponta, composta por três etapas principais:
Geração e tratamento dos dados
Enriquecimento dos dados com apoio de IA
Visualização executiva orientada à decisão

3 - Arquitetura da solução
Geração de dados (Python)
Foram gerados dados fictícios realistas de reclamações de clientes, simulando lojas, produtos, datas, estoque e comentários em linguagem natural.

4 - Pipeline de tratamento (Python + Pandas)
Os dados passaram por um pipeline que:
– Padroniza nomes de produtos
– Normaliza categorias
– Estrutura os dados para análise
– Calcula métricas operacionais

5 - Uso de IA generativa
A IA foi utilizada de forma pontual e responsável para:
– Classificar automaticamente o tipo de ocorrência (ruptura virtual, ruptura real, preço, atendimento, elogio)
– Identificar o sentimento do cliente
– Gerar um alerta operacional de ruptura quando aplicável
A IA não toma decisões sozinha. Ela atua como apoio analítico, acelerando a classificação e liberando tempo para análise humana.
6 - Armazenamento
Os dados tratados são gravados em banco PostgreSQL (Neon), simulando um ambiente de dados corporativo.
7 - Visualização (Power BI + Figma)
O dashboard foi desenhado no Figma e implementado no Power BI, com foco em leitura executiva, clareza visual e storytelling orientado a negócio.

8 - Estrutura do dashboard
O dashboard é dividido em três páginas:
8.1 Panorama Executivo
	Visão geral do cenário:
	– Total de ocorrências
	– Ocorrências negativas
	– Alertas de ruptura
	– Evolução temporal
	– Comparação entre lojas
8.2 Diagnóstico das Ocorrências e Impacto no Cliente
Análise do impacto das categorias:
– Percentual de ruptura virtual
– Peso da ruptura na insatisfação
– Comparação por loja e categoria
Alertas de Ruptura e Ação Operacional
Foco em ação:
– Produtos com maior recorrência de ruptura
– Evolução dos alertas ao longo do tempo
– Produtos críticos por loja
– Priorização operacional
Principais insights obtidos
– A ruptura virtual concentra a maior parte das ocorrências negativas
– Poucos produtos concentram grande parte dos alertas
– Existem diferenças claras entre lojas, indicando necessidade de ações localizadas
– O problema se mantém recorrente ao longo do tempo, não sendo pontual
Esses achados reforçam a importância de integrar dados operacionais, análise e visualização para apoiar decisões rápidas.
Tecnologias utilizadas
– Python (Pandas, SQLAlchemy)
– PostgreSQL (Neon)
– Power BI
– Figma (layout e design do dashboard)
– IA generativa (classificação de texto e apoio analítico)
Observação importante
Todos os dados utilizados são fictícios e foram gerados exclusivamente para fins educacionais e de portfólio.
Autor
[Matheus Rodrigues Lopes]
LinkedIn: [ https://www.linkedin.com/in/matheuslopesr/ ]
GitHub: [ https://github.com/mrlopes15 ]
