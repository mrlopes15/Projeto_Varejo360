# Varejo 360 — Monitoramento Inteligente de Ocorrências no Varejo


## 1. Contexto do problema

No varejo físico, uma das maiores fontes de insatisfação do cliente não é necessariamente a falta de vendas, mas a experiência frustrada no ponto de venda. Produtos que constam como disponíveis no sistema, mas não estão na prateleira, divergências de preço e falhas operacionais impactam diretamente a percepção do consumidor e a eficiência da operação.

O desafio está em transformar reclamações e avaliações dispersas em informações estruturadas, capazes de apoiar decisões operacionais e priorização de ações no dia a dia das lojas.

Este projeto nasce com esse objetivo: organizar, analisar e visualizar ocorrências do varejo de forma clara, prática e orientada à ação.

---

## 2. Objetivo do projeto

O Varejo 360 tem como objetivo oferecer uma visão integrada das ocorrências registradas pelos clientes, permitindo:
	* **Identificar padrões de insatisfação**;
	* **Detectar rupturas virtuais e reais**;
	* **Priorizar produtos e lojas críticas**;
	* **Apoiar decisões operacionais com dados**.

Tudo isso com foco em clareza executiva, leitura rápida e aplicabilidade prática.

---

## 3. Visão geral da solução

A solução foi estruturada em três camadas principais:
	* **Geração e tratamento de dados**;
	* **Classificação inteligente das ocorrências**;
– Visualização executiva no Power BI

O fluxo parte de dados simulados de varejo, passa por um pipeline em Python com apoio de IA generativa para classificação de ocorrências e termina em dashboards interativos que traduzem dados em decisões.

4. Uso de IA generativa no projeto

A IA generativa foi utilizada de forma controlada e objetiva, com foco em apoiar a análise, não substituí-la.

Especificamente, a IA foi aplicada para:

– Classificar automaticamente os comentários dos clientes
– Identificar o tipo de ocorrência (ruptura virtual, ruptura real, preço, atendimento ou elogio)
– Determinar o sentimento associado à avaliação
– Sinalizar alertas de ruptura virtual quando aplicável

O uso da IA aqui tem caráter analítico e operacional, funcionando como um classificador inteligente dentro do pipeline de dados.

5. Pipeline de dados (visão técnica)

O pipeline foi desenvolvido em Python e segue as seguintes etapas:

Geração de dados fictícios realistas de varejo

Padronização e normalização de produtos

Classificação das ocorrências via IA

Cálculo de métricas e indicadores

Persistência dos dados em banco PostgreSQL

Consumo dos dados pelo Power BI

Essa abordagem permite fácil reprocessamento, escalabilidade e replicação do modelo.

6. Arquitetura da solução

Tecnologias utilizadas:

– Python (pandas, SQLAlchemy)
– OpenAI API (classificação de texto)
– PostgreSQL (Neon)
– Power BI
– GitHub (versionamento)
– Figma (design do layout do dashboard)

O layout visual do dashboard foi desenhado previamente no Figma e depois implementado no Power BI, garantindo consistência visual e melhor experiência de leitura.

7. Dashboard — Panorama Executivo

Esta página oferece uma visão macro da operação.

Principais elementos:

– Total de ocorrências registradas
– Quantidade de ocorrências negativas
– Alertas de ruptura identificados
– Custo estimado do processamento analítico
– Distribuição das ocorrências por categoria
– Comparativo de ocorrências negativas por loja
– Evolução temporal das ocorrências

Objetivo: permitir que um gestor entenda rapidamente onde estão os principais pontos de atenção.

(Insira aqui a imagem da Página 1 do dashboard)

8. Dashboard — Diagnóstico das Ocorrências e Impacto no Cliente

Nesta etapa, o foco é entender o impacto das ocorrências na experiência do cliente.

Principais análises:

– Percentual de ocorrências relacionadas à ruptura virtual
– Comparativo entre ruptura virtual, ruptura real e outros fatores
– Distribuição das ocorrências por loja e categoria
– Identificação do principal fator de insatisfação

Insight-chave: a ruptura virtual concentra a maior parte da insatisfação do cliente, indicando falhas entre o estoque sistêmico e a operação de loja.

(Insira aqui a imagem da Página 2 do dashboard)

9. Dashboard — Alertas de Ruptura e Ação Operacional

Esta página é orientada à ação.

Principais recursos:

– Produtos com maior número de alertas de ruptura
– Top ofensores (produtos mais críticos)
– Evolução dos alertas ao longo do tempo
– Matriz de produtos críticos por loja

O objetivo é apoiar decisões práticas, como:

– Reposição prioritária
– Revisão de processos logísticos
– Ajustes de abastecimento por loja

(Insira aqui a imagem da Página 3 do dashboard)

10. Principais insights do projeto

– A ruptura virtual representa mais de 60% das ocorrências negativas
– Determinados produtos concentram alertas recorrentes
– Existem diferenças claras entre lojas no perfil de ocorrência
– A análise temporal indica recorrência do problema, não eventos isolados

Esses insights permitem sair da reação pontual e avançar para uma gestão preventiva.

11. Estrutura do repositório
├── src/
│   ├── gerar_dados.py
│   └── pipeline_main.py
├── sql/
│   ├── create_table_analise_varejo360.sql
│   ├── ruptura_virtual.sql
│   └── sentimento_loja.sql
├── dashboard/
│   └── Varejo_360.pbix
├── assets/
│   └── imagens do dashboard
├── README.md
├── requirements.txt

12. Próximos passos e evoluções possíveis

– Conectar dados reais de vendas e estoque
– Integrar indicadores financeiros
– Criar alertas automáticos
– Expandir o uso de IA para análise preditiva

13. Autor

Matheus Rodrigues Lopes
[Matheus Rodrigues Lopes]
LinkedIn: [ https://www.linkedin.com/in/matheuslopesr/ ]
GitHub: [ https://github.com/mrlopes15 ]
