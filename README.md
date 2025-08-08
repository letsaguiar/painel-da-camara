# Painel da Câmara — Despesas parlamentares (CEAP)

**Transparência prática sobre gastos parlamentares.**
Explore por deputado, partido, UF e período — com gráficos didáticos e links para os comprovantes.

**Status:** v0.1.0 (conteúdo & identidade) • **Licença:** MIT • **Analytics:** nenhum (apenas logs técnicos)

---

## Sumário

* [1. O que é](#1-o-que-é)
* [2. Por que existe](#2-por-que-existe)
* [3. Para quem](#3-para-quem)
* [4. Como funciona (visão do produto)](#4-como-funciona-visão-do-produto)
* [5. Dashboard (rótulos e IA)](#5-dashboard-rótulos-e-ia)
* [6. Branding & Identidade](#6-branding--identidade)
* [7. Acessibilidade](#7-acessibilidade)
* [8. Dados & Metodologia](#8-dados--metodologia)
* [9. Roadmap](#9-roadmap)
* [10. Governança & Contribuição](#10-governança--contribuição)
* [11. Licença](#11-licença)
* [12. Contato](#12-contato)

---

## 1. O que é

O **Painel da Câmara** é uma plataforma aberta para consultar e visualizar as **despesas parlamentares (CEAP)** da Câmara dos Deputados. A experiência foca em **clareza**, **filtros úteis** e **links para os comprovantes**.

---

## 2. Por que existe

* **Transparência acionável:** transformar planilhas volumosas em respostas objetivas.
* **Jornalismo e controle social:** facilitar investigações e análises rápidas.
* **Educação cívica:** tornar os dados compreensíveis para qualquer pessoa.

---

## 3. Para quem

* **Jornalistas e pesquisadores** que precisam de recortes rápidos e confiáveis.
* **Cidadãos** interessados em acompanhar gastos por bancada/UF.
* **Gestores públicos** que desejam referências de usabilidade e prestação de contas.

---

## 4. Como funciona (visão do produto)

* **Fonte oficial:** arquivos anuais da CEAP (CSV/ZIP), com atualização diária.
* **Filtros globais:** Período, UF, Partido, Deputado.
* **Visões principais:** série mensal de gastos, ranking de fornecedores e tabela detalhada com comprovantes.
* **Transparência:** cada registro aponta para o **documento** original.

---

## 5. Dashboard (rótulos e IA)

### 5.1 Filtros (topo)

* **Período:** Mês/Ano (ex.: jan–dez/2025)
* **UF:** sigla (ex.: SP, MG)
* **Partido:** sigla (ex.: PT, PL, UNIÃO…)
* **Deputado:** nome parlamentar

**Estado vazio:** “Sem resultados para este filtro. Ajuste o período ou selecione outro partido.”
**Erro de carregamento:** “Não foi possível carregar os dados agora. Tente novamente mais tarde.”

### 5.2 KPIs (cartões)

1. **Total no período**
2. **Média por deputado**
3. **Top tipo de despesa**
4. **Nº de documentos**

### 5.3 Gráficos

* **Gasto mensal — CEAP** (barras; eixo X = mês, Y = valor)
* **Fornecedores com maior volume** (barras horizontais; top 10)

### 5.4 Tabela (colunas)

* **Deputado** • **Partido** • **UF** • **Mês/Ano** • **Tipo de despesa** • **Fornecedor** • **Valor líquido** • **Documento**

### 5.5 Perguntas que o painel responde

* Quanto gastou **cada partido** nos últimos 12 meses?
* Qual **UF** teve maior gasto médio por deputado?
* Quais são os **top fornecedores** por volume no período selecionado?
* Como evoluiu o gasto de um **deputado específico** ao longo do ano?

---

## 6. Branding & Identidade

### 6.1 Tom de voz

Direto, factual e acessível. Títulos curtos; evitar jargão técnico.

### 6.2 Paleta de cores (tokens)

| Token             | Hex       | Uso principal              |
| ----------------- | --------- | -------------------------- |
| `brand/primary`   | `#0B6B43` | Ações primárias, header    |
| `brand/secondary` | `#0D3B66` | Destaques, links           |
| `accent/warn`     | `#F2C14E` | Indicadores/alertas suaves |
| `text/default`    | `#2E2E2E` | Texto padrão               |
| `text/muted`      | `#6B7280` | Texto secundário           |
| `bg/base`         | `#F8FAFC` | Plano de fundo             |

**Contraste mínimo:** WCAG AA (verificar títulos e botões ≥ 4.5:1).

### 6.3 Tipografia

* **Títulos:** Public Sans (ou Inter) — pesos 600–700
* **Texto:** Source Sans 3 (ou Noto Sans) — pesos 400–500
* **Hierarquia sugerida:** H1 32–40 • H2 24–28 • H3 18–20 • Corpo 14–16

### 6.4 Logo, ícones e imagens

* **Logo (brief):** ícone minimalista do prédio do Congresso com barras horizontais representando “dados”. Versões: mono (clara/escura) e bicolor (verde/azul).
* **Favicon:** redução do ícone em 32×32.
* **App icon:** 512×512 versão bicolor.
* **OG image (redes):** 1200×630, fundo claro, título “Painel da Câmara”, subtítulo “Despesas parlamentares — CEAP”, logomarca à esquerda.
* **Alt texts:**

  * Logo: “Logomarca do Painel da Câmara.”
  * Hero: “Ilustração do Congresso com cartões de dados e gráfico de barras.”
  * OG: “Imagem de compartilhamento do Painel da Câmara.”

### 6.5 Landing — microcopy

* **Hero title:** **Veja quanto sua bancada gasta.**
* **Hero subtitle:** **Explore despesas por deputado, partido, UF e período. Links para cada comprovante.**
* **CTA primário:** **Abrir o painel**
* **CTA secundário:** **Como funcionam os dados**
* **Seção — O que você encontra**

  1. Séries mensais por partido/UF
  2. Ranking de fornecedores e tipos de despesa
  3. Links diretos para documentos
* **Seção — Metodologia**
  Dados oficiais (CEAP), atualização diária, coleta por arquivos anuais CSV/ZIP.
* **Seção — Transparência**
  Cadastro do deputado, tipo de despesa, fornecedor, valor líquido e documento — tudo em um só lugar.
* **Rodapé:** Projeto aberto. Contribua no GitHub.

---

## 7. Acessibilidade

* Navegação por teclado e rótulos claros nos filtros.
* Contraste **AA** em botões, links e textos.
* Estados visuais e textuais para **carregando**, **erro** e **sem resultados**.
* Textos alternativos (alt) em todas as imagens.
* Tamanho mínimo de fonte recomendado: 14 px no corpo.

---

## 8. Dados & Metodologia

### 8.1 Fontes

* **CEAP — Câmara dos Deputados** (arquivos anuais CSV/ZIP).
* Metadados complementares de deputados poderão ser agregados conforme disponibilidade pública.

### 8.2 Atualização

* **Diária** (conforme publicação dos arquivos oficiais).
* Registro de atualização e eventuais falhas documentados em **/metodologia**.

### 8.3 Dicionário (campos mínimos v1)

* `ideCadastro` (id do parlamentar)
* `txNomeParlamentar` (nome parlamentar)
* `sgUF` (UF)
* `sgPartido` (partido)
* `numAno`, `numMes` (período)
* `numSubCota` / `txtDescricao` (tipo de despesa)
* `txtFornecedor` / `txtCNPJCPF` (fornecedor)
* `vlrLiquido` (valor efetivo)
* `urlDocumento` (link do comprovante)

### 8.4 Limitações e notas de qualidade

* Divergências de **partido/UF** e nomes ao longo do tempo podem ocorrer.
* Homônimos e normalização de fornecedores exigem cuidado.
* Valores podem sofrer ajustes posteriores; sempre referenciar o documento.

### 8.5 Ética e transparência

* Uso responsável de dados públicos.
* Nenhum dado sensível exposto.
* Link para a **fonte original** em cada registro sempre que disponível.

---

## 9. Roadmap

### Sprint 1 — Kickoff & Conteúdo (07–13 ago 2025)

* Branding & conteúdo v1 publicados (este README, /sobre, /metodologia).
* Contratos de **dados CEAP** e **API `/despesas`** definidos (parâmetros, resposta, paginação, ordenação, erros).
* Imagem **OG** e pacote de ícones especificados (briefs e alt).

### Sprint 2 — Planejamento de ingestão CEAP & painel (14–20 ago 2025)

* Estratégia de ingestão com **arquivos anuais CSV/ZIP** (idempotência, “raw” + normalizado).
* Filtros finais por caso de uso; exemplos de consulta e resposta.
* Página **/dados** com links oficiais por ano.

### Versão 1.0.0 (posterior)

* Deploy público, autenticação por token (áreas protegidas), rate limit, observabilidade, melhoria de UX e documentação de API com exemplos.

---

## 10. Governança & Contribuição

### Papéis

* **Product Owner / Gestão:** responsável por escopo, priorização e qualidade.
* **Colaboração externa:** melhorias de conteúdo, design e documentação são bem-vindas.

### Fluxos

* **Issues:** use rótulos “conteúdo”, “dados”, “design”, “infra” e “bug”.
* **Propostas:** descreva objetivo, impacto, DoD e riscos.
* **PRs:** pequenos e focados; inclua resumo, screenshots (quando visual) e links de referência.

### Código de conduta (resumo)

* Comunicação respeitosa; foco em fatos e evidências; zero tolerância a assédio.

---

## 11. Licença

**MIT** — código aberto e uso permitido com atribuição.
Os **dados** seguem os termos da Câmara dos Deputados.

---

## 12. Contato

* **Projeto:** Painel da Câmara
* **Assuntos:** dúvidas, sugestões, correções de conteúdo e acessibilidade
* **Canal:** abrir issue pública no repositório (quando disponível)

---

### Anexos (para o repositório)

* `/assets/logo.svg` • `/assets/favicon-32.png` • `/assets/app-icon-512.png` • `/assets/og.png`
* `/docs/sobre.md` • `/docs/metodologia.md` • `/docs/dados.md` (com links oficiais)
* `CHANGELOG.md` (iniciar em v0.1.0 — “Conteúdo & identidade publicados”)