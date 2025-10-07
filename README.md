📋 Sobre o Projeto
Este repositório contém uma solução avançada de matching inteligente desenvolvida em Python para identificar e relacionar automaticamente clientes, produtos e oportunidades de negócio a partir de múltiplas fontes de dados corporativas. O sistema foi projetado para atender demandas específicas de equipes comerciais que necessitam cruzar informações entre diferentes bases como List Mapping, All Products e Business Group.

🎯 Objetivo Principal
Automatizar o processo de identificação de clientes estratégicos e suas relações com produtos e subsidiárias, utilizando técnicas de fuzzy matching e análise contextual para garantir precisão mesmo quando os nomes variam entre diferentes sistemas.

🔧 Funcionalidades Principais
🎯 Busca Prioritária por Palavras-Chave
Identificação automática de clientes relacionados à PepsiCo e suas subsidiárias

Verificação contextual rigorosa para evitar falsos positivos

Análise em múltiplas camadas: Global Ultimate, Domestic Ultimate e Account Name

🔍 Matching Inteligente com Tolerância a Variações
Fuzzy Matching com múltiplos algoritmos (Token Set, Jaro-Winkler, Cosine Similarity)

Normalização avançada de textos (remoção de sufixos corporativos, países, caracteres especiais)

Suporte a diferentes limiares de similaridade configuráveis

📊 Integração Multi-Fonte
Cruzamento automático entre List Mapping × Business Group × All Products

Identificação de oportunidades de venda relacionadas a cada cliente

Validação de produtos compatíveis com o portfólio da empresa

🏗️ Arquitetura em Camadas
Camada 0: Busca prioritária por palavras-chave específicas

Camada 1: Matching Global Ultimate Name × Subsidiárias LAD

Camada 2: Matching Domestic Ultimate Name × Todas as Subsidiárias

Camada 3: Matching Account Name × Subsidiárias restantes

Camada 4: Integração com All Products

Camada 5: Validação de produtos

💼 Casos de Uso
Para Equipes de Vendas
Identificar quais clientes são subsidiárias da PepsiCo

Descobrir oportunidades de venda não exploradas

Entender o relacionamento hierárquico entre clientes

Para Análise Comercial
Mapear o market share por subsidiária

Identificar gaps no portfólio de produtos

Analisar performance por região/segmento

Para Gestão Estratégica
Visualizar a rede completa de clientes corporativos

Planejar estratégias de expansão baseadas em dados

Otimizar alocação de recursos comerciais

🛠️ Tecnologias e Bibliotecas
Python 3.x - Linguagem base

pandas - Manipulação de dados

rapidfuzz/fuzzywuzzy - Algoritmos de fuzzy matching

scikit-learn - Similaridade por cosine

unidecode - Normalização de caracteres

pyxlsb - Leitura de arquivos Excel binários

xlsxwriter - Exportação de resultados

📈 Fluxo de Processamento
Carregamento - Leitura dos arquivos fonte (List Mapping, All Products, Business Group)

Normalização - Padronização de nomes e remoção de ruído

Busca Prioritária - Identificação de clientes PepsiCo via palavras-chave

Matching em Camadas - Cruzamento progressivo com tolerância a variações

Integração - Consolidação com dados de produtos e oportunidades

Exportação - Geração de relatório completo em Excel
