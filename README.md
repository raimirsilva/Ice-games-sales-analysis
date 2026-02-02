# 🎮 Ice Games Sales Analysis

**Análise de Dados de Vendas de Videogames para Planejamento Estratégico**

***

## 📋 Sobre o Projeto

Este projeto de análise de dados foi desenvolvido como parte do bootcamp TripleTen de Data Analytics. O objetivo é identificar padrões que determinam o sucesso de videogames no mercado global, permitindo à loja online **Ice** planejar campanhas publicitárias eficazes para 2017.

Através da análise de dados históricos de vendas, avaliações de usuários e especialistas, gêneros e plataformas, este projeto demonstra habilidades em **análise exploratória de dados**, **visualização**, **testes estatísticos** e **storytelling com dados**.

***

## 🎯 Objetivos

- Identificar padrões que determinam o sucesso comercial de videogames
- Analisar a evolução das plataformas de jogos ao longo do tempo
- Compreender diferenças regionais no comportamento de consumo (América do Norte, Europa e Japão)
- Avaliar o impacto de avaliações críticas e de usuários nas vendas
- Testar hipóteses estatísticas sobre avaliações de plataformas e gêneros
- Fornecer insights acionáveis para campanhas de marketing em 2017

***

## 🗂️ Estrutura do Projeto

### **Etapa 1: Carregamento e Exploração Inicial**
- Importação do dataset `games.csv`
- Análise preliminar da estrutura dos dados
- Identificação de características e limitações do conjunto de dados

### **Etapa 2: Preparação dos Dados**
- **Padronização** de nomes de colunas (lowercase)
- **Conversão** de tipos de dados apropriados
- **Tratamento de valores ausentes** com análise de padrões e justificativas
- Gestão de casos **TBD** (*to be determined*)
- Criação de coluna de **vendas totais globais**

### **Etapa 3: Análise Exploratória de Dados (EDA)**
- Análise temporal de lançamentos de jogos
- Evolução de vendas por plataforma ao longo dos anos
- Identificação de plataformas em ascensão e declínio
- Seleção do período relevante para modelagem (2017)
- Análise de plataformas potencialmente lucrativas
- Box plots de vendas globais por plataforma
- Correlação entre avaliações (críticos e usuários) e vendas
- Análise de distribuição por gênero

### **Etapa 4: Perfil Regional de Usuários**
Análise comparativa para **América do Norte (NA)**, **Europa (EU)** e **Japão (JP)**:
- Top 5 plataformas por região
- Top 5 gêneros por região
- Impacto das classificações ESRB nas vendas regionais
- Variações de market share entre regiões

### **Etapa 5: Testes de Hipóteses**
**Hipótese 1:** Classificações médias de usuários são iguais entre Xbox One e PC

**Hipótese 2:** Classificações médias de usuários diferem entre gêneros Action e Sports

- Formulação de hipóteses nulas e alternativas
- Definição do nível de significância (α)
- Aplicação de testes estatísticos apropriados
- Interpretação dos resultados

### **Etapa 6: Conclusões e Recomendações**
- Síntese dos principais insights
- Recomendações estratégicas para campanhas de 2017
- Limitações do estudo e sugestões para análises futuras

***

## 📊 Dataset

### **Fonte**
`/datasets/games.csv`

### **Descrição das Colunas**

| Coluna | Descrição |
|--------|-----------|
| `Name` | Nome do jogo |
| `Platform` | Plataforma (Xbox, PlayStation, PC, etc.) |
| `Year_of_Release` | Ano de lançamento |
| `Genre` | Gênero do jogo |
| `NA_sales` | Vendas na América do Norte (milhões USD) |
| `EU_sales` | Vendas na Europa (milhões USD) |
| `JP_sales` | Vendas no Japão (milhões USD) |
| `Other_sales` | Vendas em outros países (milhões USD) |
| `Critic_Score` | Pontuação de críticos (máximo 100) |
| `User_Score` | Pontuação de usuários (máximo 10) |
| `Rating` | Classificação ESRB |

**⚠️ Nota:** Dados de 2016 podem estar incompletos devido à proximidade temporal.

***

## 🛠️ Tecnologias Utilizadas

### **Bibliotecas Principais**
- **Pandas** — Manipulação e análise de dados
- **NumPy** — Operações numéricas
- **Matplotlib & Seaborn** — Visualização de dados
- **SciPy** — Testes estatísticos
- **Jupyter Notebook** — Desenvolvimento e documentação

***

## 🚀 Como Executar

### **Pré-requisitos**
```bash
python >= 3.8
jupyter notebook
pandas
numpy
matplotlib
seaborn
scipy
```

### **Instalação**
```bash
# Clone o repositório
git clone https://github.com/raimirsilva/Ice-games-sales-analysis.git

# Navegue até o diretório
cd Ice-games-sales-analysis

# Instale as dependências
pip install -r requirements.txt

# Inicie o Jupyter Notebook
jupyter notebook
```

### **Execução**
Abra o arquivo `Ice_games_analysis.ipynb` e execute as células sequencialmente.

***

## 📈 Principais Insights

*Esta seção será atualizada com os principais achados após a conclusão da análise.*

### **Plataformas**
- Evolução: identificou-se um ciclo de vida médio de 6 a 8 anos para consoles; em 2016, o mercado vive o declínio acelerado da 7ª geração (PS3, Xbox 360) e a consolidação definitiva da 8ª geração.
- Market Leaders: o PS4 consolidou-se como líder global, seguido pelo Xbox One (forte na América do Norte); no Japão, o 3DS mantém a liderança absoluta no segmento portátil.

### **Gêneros**
- Lucratividade (ROI): embora Action tenha o maior volume total, gêneros como Shooter, Sports e Platform apresentam melhor equilíbrio entre vendas médias e saturação, oferecendo maior potencial de retorno sobre investimento.
- Preferências: o gênero Action é onipresente, mas o sucesso comercial em 2017 depende da escolha correta da plataforma para cada nicho.

### **Avaliações**
- Impacto: notas de críticos acima de 7.0 possuem correlação positiva com o aumento de vendas, servindo como um selo de qualidade que impulsiona o desempenho comercial.
- Correlações: a pontuação dos especialistas tem uma influência estatística muito mais significativa nas vendas do que a avaliação dos usuários, que apresenta correlação fraca ou nula.

### **Regionalização**
- Diferenças regionais: a América do Norte e Europa possuem perfis similares (foco em consoles de mesa e jogos M-rated), enquanto o Japão é um mercado distinto, priorizando consoles portáteis e conteúdo de classificação E/T-rated (RPGs e jogos familiares).

***

## 📝 Metodologia

### **Tratamento de Dados**
- Aplicação de técnicas de data cleaning apropriadas
- Justificativa documentada para decisões de imputação
- Análise de missingness patterns

### **Análise Estatística**
- Testes paramétricos e não-paramétricos quando apropriado
- Verificação de pressupostos estatísticos
- Interpretação contextualizada dos resultados

### **Visualização**
- Gráficos informativos e esteticamente agradáveis
- Legendas e títulos descritivos
- Uso de cores para destacar insights

***

## 🎓 Aprendizados

Este projeto demonstra competências em:

- **Limpeza e preparação de dados** com tratamento criterioso de missing values  
- **Análise exploratória de dados (EDA)** com visualizações informativas  
- **Análise temporal** e identificação de tendências  
- **Segmentação regional** e análise comparativa  
- **Testes de hipóteses estatísticas** com interpretação adequada  
- **Storytelling com dados** e comunicação de insights  
- **Documentação técnica** clara e profissional  

***

## 👤 Autor

**[Raimir Silva]**

- GitHub: [@raimirsilva](https://github.com/raimirsilva)
- LinkedIn: [Raimir Silva](https://linkedin.com/in/raimir-silva)
- Email: raimir@proton.me

***

## 📄 Licença

Este projeto foi desenvolvido como parte do bootcamp **TripleTen Data Analytics** para fins educacionais e de portfólio.

***

**⭐ Se este projeto foi útil para você, considere dar uma estrela no repositório!**
