# Relatório de Estágio Supervisionado — UFAC

Relatório de estágio de **Marcos Vinícius Moraes Costa**, referente ao desenvolvimento de um sistema web para gestão e controle de uso da Sala de Informática da Biblioteca Central da Universidade Federal do Acre (UFAC), sob orientação acadêmica de **Laura Costa Sarkis**.

A organização dos capítulos segue o documento **ModelodeRelatoriodeEstagio_template.docx**, disponibilizado pela UFAC. A composição gráfica utiliza a classe **abnTeX2** e a personalização local `abntex2-UFAC.sty`.

## Arquivos

- `relatorio_estagio.tex`: arquivo principal, com capa, folha de rosto, elementos pré-textuais, sumário e referências;
- `pre-textuais.tex`: termo de aprovação, dedicatória, agradecimentos, epígrafe, resumo, abstract, listas de figuras/quadros/tabelas e siglas;
- `capitulos/01-introducao.tex`: problema, objetivos, justificativa, metodologia e organização do estudo;
- `capitulos/02-fundamentacao.tex`: embasamento teórico e referências do projeto acadêmico;
- `capitulos/03-estagio.tex`: instituição, organização de trabalho, atividades e resultados técnicos;
- `referencias_estagio.bib`: obras efetivamente citadas;
- `abntex2-UFAC.sty` e `figuras/exefig.eps`: personalização visual original da UFAC.

O exemplo do estágio de outra organização e seus arquivos compilados antigos foram retirados deste repositório. A manutenção do estilo UFAC não representa aproveitamento daquele conteúdo.

## Compilação

No Overleaf, configure **`relatorio_estagio.tex` como arquivo principal** e selecione o compilador **pdfLaTeX**. O projeto utiliza BibTeX para referências e `epstopdf` para o brasão em EPS.

Para compilar localmente em uma instalação LaTeX compatível:

```sh
pdflatex -shell-escape relatorio_estagio.tex
bibtex relatorio_estagio
pdflatex -shell-escape relatorio_estagio.tex
pdflatex -shell-escape relatorio_estagio.tex
```

## Fontes do conteúdo

- [Projeto acadêmico de estágio](https://github.com/MarcosVini753/Projeto_Estagio_UFAC)
- [Documentação e implementação do sistema (branch dev)](https://github.com/MarcosVini753/estagio/tree/dev)
- Fichas de controle e frequência do estágio supervisionado
- Modelo Word institucional de relatório de estágio

## Pendências para conclusão

1. Confirmar dados institucionais e eventual organograma oficial com a supervisão.
2. Inserir capturas de tela reais, diagramas selecionados e fontes das ilustrações.
3. Conferir evidências de testes e de validação com a biblioteca; não presumir implantação em produção.
4. Redigir o capítulo de considerações finais e recomendações.
5. Preencher os placeholders de aprovação (data e banca), dedicatória, agradecimentos, epígrafe, resumo, abstract e palavras-chave em `pre-textuais.tex`.
6. Revisar as listas automáticas de figuras, quadros e tabelas quando houver elementos com legendas nos capítulos.

**Nota de escopo:** a aplicação documentada ainda não possui autenticação institucional real, fila de espera, relatório semanal específico ou interface própria funcional para o Administrador. O relatório não apresenta essas funcionalidades como implementadas.

## Elementos antes do sumário

O arquivo `pre-textuais.tex` preserva a ordem do modelo Word: termo de aprovação, dedicatória, agradecimentos, epígrafe, resumo, abstract, listas de figuras, quadros e tabelas, além da lista de siglas. Os campos entre colchetes são **placeholders**, não informações definitivas. As listas de ilustrações são geradas pelo LaTeX conforme figuras, quadros e tabelas forem incluídos. Para um quadro, use o ambiente `quadro` com `\\caption{...}`.
