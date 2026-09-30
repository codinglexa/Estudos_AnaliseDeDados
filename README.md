# 🎮 League of Legends — Análise de Dados da Selva (EUW)

> **Análise exploratória do desempenho de caçadores (Jungle) no servidor Europeu Ocidental (EUW), mapeando métricas de impacto por elo.**

---

## 📌 Visão Geral

Este projeto analisa **1.625 partidas** de League of Legends com foco na rota da Selva (*Jungle*). O objetivo principal é compreender quais fatores operacionais (objetivos, KDA, farm, controle de visão e escolhas) mais impactam a taxa de vitória ao longo dos diferentes ranques do jogo.

---

## 💡 Questões de Pesquisa

* **Métricas por Elo:** Variação do comportamento tático entre os ranques.
* **Peso dos Objetivos:** A relevância de Dragões, Barões e Arautos para fechar o jogo.
* **KDA vs. Dano:** Qual métrica possui maior peso na vitória?
* **Recursos:** O impacto do farm e ouro acumulado.
* **Visão:** Variação no controle da névoa de guerra por divisão.
* **Meta:** Campeões e runas de melhor desempenho.

---

## 📊 Estrutura dos Dados

Os dados foram tratados e padronizados no Pandas para refletir as seguintes categorias:

| Categoria | Métricas Incluídas |
| :--- | :--- |
| **Identificação** | `Ranque`, `Campeão`, `Runa`, `ID da Partida` |
| **Resultado** | `Vitória` (1/0), `Duração da Partida` |
| **Combate** | `Kills`, `Mortes`, `Assistências`, `KDA`, `Participações (KP)` |
| **Recursos** | `Farm`, `Farm por Minuto`, `Ouro`, `Dano`, `% Dano`, `Dano Sofrido` |
| **Visão** | `Visão`, `Wards`, `Wards Destruídas`, `Wards de Controle` |
| **Objetivos** | `Dragões`, `Barons`, `Arautos`, `Torres` (e % de participação) |

---

## 🔍 Destaques & Insights

### 📈 Distribuição de Partidas por Elo
```text
├── Bronze:    285
├── Prata:     255
├── Ferro:     251
├── Ouro:      238
├── Diamante:  203
├── Esmeralda: 200
└── Platina:   193
````
### 🐲 O Peso do Dragão: A conquista de Dragões apresentou a maior correlação direta com a vitória entre todas as estatísticas avaliadas.

### 🎯 KDA x Dano Total: Ter um KDA sólido correlaciona-se mais fortemente com a vitória do que apresentar apenas números altos de dano total.

### ⏳ Duração das Partidas:

Jogos Mais Longos: Ferro, Bronze e Platina.

Jogos Mais Rápidos: Prata, Esmeralda e Diamante.

### 🏆 Campeões em Destaque:

Kayn: Maior número absoluto de vitórias na amostra.

Briar: Destaque em taxa de vitória nos elos Bronze e Diamante.

### 🛠️ Tecnologias & Bibliotecas
Linguagem: Python 3.x

Análise de Dados: pandas, numpy

Visualização: matplotlib

Ambiente: Google Colab / Jupyter Notebook

### 🚀 Como Executar
Clone o repositório:
````
Bash
git clone [https://github.com/seu-usuario/lol-jungle-analysis.git](https://github.com/seu-usuario/lol-jungle-analysis.git)
cd lol-jungle-analysis
````

Instale as dependências:

````
Bash
pip install pandas numpy matplotlib

````
Execute o Notebook:

````
Abra o arquivo ProjetoAnáliseDeDados_LeagueOfLegends.ipynb em seu ambiente preferido (Jupyter ou Colab).
````
