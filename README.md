# Mestrado em Letras - UFT (Porto Nacional)

Repositório destinado à organização de materiais, artigos e produção da dissertação do Mestrado Acadêmico em Letras da Universidade Federal do Tocantins (Câmpus Porto Nacional).

## Estrutura
O repositório segue uma organização cronológica por semestres e temática por disciplinas.

- **Artigos:** Contém fichamentos e rascunhos de artigos em LaTeX (modelo ABNT).
- **Apresentacoes:** Slides para seminários (modelo Beamer UFT).
- **Dissertacao:** (No 4º Semestre) Projeto completo configurado com abnTeX2 adaptado para normas da UFT.

## Como Compilar (LaTeX)
Certifique-se de ter uma distribuição TeX instalada (TeX Live, MiKTeX) e o pacote `abntex2`.

Para compilar a dissertação:
```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```