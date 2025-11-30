# Mestrado em Letras - UFT (Porto Nacional)

![Status](https://img.shields.io/badge/Status-Em_Desenvolvimento-yellow)
![LaTeX](https://img.shields.io/badge/LaTeX-ABNT2-green)
![Instituição](https://img.shields.io/badge/UFT-Porto_Nacional-blue)

Bem-vindo ao repositório oficial da organização **wbn-letras**. Este ambiente foi criado para centralizar, versionar e padronizar a produção acadêmica durante o **Programa de Pós-Graduação em Letras (PPG-Letras)** da Universidade Federal do Tocantins (Câmpus Porto Nacional).

Aqui você encontrará *templates*, fichamentos e a estrutura completa da dissertação formatada em LaTeX, seguindo rigorosamente as normas da ABNT e as diretrizes da UFT.

---

## 🏛️ Sobre o Programa (PPG-Letras)

O Mestrado Acadêmico em Letras da UFT (Porto Nacional) está estruturado em duas grandes áreas de concentração. Este repositório está preparado para atender demandas de ambas:

### 1. Estudos Linguísticos
*   Abordagens de Análise Linguística
*   Linguística Aplicada
*   Texto, Discurso e História
*   Língua Brasileira de Sinais (Libras)

### 2. Estudos Literários
*   Literatura, História e Imaginário
*   Teoria, Crítica e Comparatismo

---

## 📂 Estrutura do Repositório

A organização dos diretórios segue a cronologia dos 24 meses do curso:

| Diretório | Conteúdo Principal |
| :--- | :--- |
| **01_Primeiro_Semestre/** | Disciplinas obrigatórias do núcleo comum. Fichamentos e artigos finais das matérias teóricas. |
| **02_Segundo_Semestre/** | Disciplinas específicas da Linha de Pesquisa e Seminários de Orientação I. |
| **03_Terceiro_Semestre/** | Qualificação da Dissertação. Slides em `Beamer` para a defesa da qualificação. |
| **04_Quarto_Semestre/** | **Dissertação Final**. Contém o projeto completo configurado com `abntex2`. |

> **Nota:** Todos os documentos `.tex` já estão configurados com pré-textuais, citações e referências bibliográficas automáticas.

---

## 🛠️ Guia de Uso (LaTeX)

Para garantir a compilação correta dos documentos, certifique-se de que seu ambiente possui:
*   **Distribuição TeX:** [TeX Live](https://www.tug.org/texlive/) (Linux/Windows) ou [MacTeX](https://www.tug.org/mactex/) (macOS).
*   **Editor Sugerido:** VS Code (com extensão *LaTeX Workshop*) ou Overleaf.

### Como Compilar (Terminal)
Utilize a sequência abaixo para garantir que índices e bibliografias sejam gerados corretamente:

```bash
# 1. Primeira compilação
pdflatex main.tex

# 2. Compilação das referências bibliográficas
bibtex main

# 3. Consolidação dos links e índices
pdflatex main.tex
pdflatex main.tex