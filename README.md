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

## 📂 Estrutura de Diretórios

O projeto está organizado cronologicamente para refletir a jornada acadêmica do mestrado (24 meses). Abaixo segue a árvore de diretórios atualizada:

```text
mestrado-letras/
│
├── 📜 gerar_mestrado.py         # Script de automação (Scaffolding)
├── 📄 README.md                 # Documentação do repositório
│
├── 📁 01_Primeiro_Semestre/
│   ├── 01_Metodologia_da_Pesquisa/
│   |   ├── 📂 Apresentacoes/    # Slides (.tex + Beamer)
│   |   └── 📂 Artigos/          # Papers finais da disciplina
│   ├── 02_Historia_do_Pensamento_Linguistico/
│   |   ├── 📂 Apresentacoes/    # Slides (.tex + Beamer)
│   |   └── 📂 Artigos/          # Papers finais da disciplina
│   ├── 03_Analise_do_Discurso/
│   |   ├── 📂 Apresentacoes/    # Slides (.tex + Beamer)
│   |   └── 📂 Artigos/          # Papers finais da disciplina
│   └── 04_Seminarios_Linguisticos/
│       ├── 📂 Apresentacoes/    # Slides (.tex + Beamer)
│       └── 📂 Artigos/          # Papers finais da disciplina
│
├── 📁 02_Segundo_Semestre/
│   ├── 01_Seminario_de_Pesquisa_I/
│   └── 02_Topicos_de_Teoria_da_Literatura/
│
├── 📁 03_Terceiro_Semestre/
│   ├── 01_Seminario_de_Pesquisa_II/
│   └── 02_Literatura_Historia_e_Imaginario/
│
└── 📁 04_Quarto_Semestre/       # Reta Final
    ├── 01_Docencia_Orientada/
    └── 02_Escrita_da_Dissertacao/
        ├── 📂 Apresentacoes/    # Slides da Defesa
        ├── 📂 Artigos/          # Artigos derivados
        └── 📂 Dissertacao/      # O Texto Final (main.tex)
```

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
