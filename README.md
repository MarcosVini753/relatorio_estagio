# Relatório de estágio — UFAC

Projeto LaTeX de relatório de estágio adaptado por Christopher Ric Coelho Saar com base no template de TCC de Sistemas de Informação da UFAC.

## Compilação no Overleaf

Defina `UFAC-modelo-TCC.tex` como arquivo principal e escolha **pdfLaTeX**. A classe é `abntex2`, com o arquivo local `abntex2-UFAC.sty`. A bibliografia utiliza `abntex2cite` (BibTeX).

O brasão da capa (`figuras/exefig.eps`) foi recuperado do [modelo da UFAC](https://github.com/mlimeira/ufac_si_template_tcc); a conversão EPS → PDF é feita por `epstopdf` durante a compilação.

## Imagens pendentes

Estas 18 imagens são referenciadas no documento original, mas não constavam do repositório. O comando `\incluirfigura` exibe um marcador **Imagem pendente** quando o arquivo não existe. Quando você enviar a imagem verdadeira para o caminho indicado, ela aparecerá automaticamente no PDF.

- `figuras/cliente.png`
- `figuras/ppi-logo.png`
- `figuras/organograma.png`
- `figuras/fluxo_demanda.png`
- `figuras/proofOfConcept.png`
- `figuras/user.model.png`
- `figuras/create.user.controller.png`
- `figuras/user.routes.png`
- `figuras/button-component-example.png`
- `figuras/buttons-parents-component-example.png`
- `figuras/useState-example.png`
- `figuras/state-usage-example.png`
- `figuras/axios-request-example.png`
- `figuras/customers.png`
- `figuras/home.png`
- `figuras/schedule.png`
- `figuras/details-tasks.png`
- `figuras/req/REQ/Documento de Requisitos de Software - 2PI ESTUDIO_page-0001.jpg`

**Atenção:** os marcadores não são imagens substitutas. Recupere os arquivos originais ou adapte/remova as figuras correspondentes ao escrever seu próprio relatório.

## Bibliografia

`referencias.bib` contém registros bibliográficos, mas o texto de exemplo não usa `\cite` nem `\citeonline`. O aviso `Empty thebibliography environment` é esperado até que citações válidas sejam incluídas. Evite adicionar `\nocite{*}`, que geraria uma lista de obras não necessariamente citadas.

O texto ainda contém dados pessoais do autor original e trechos `Lorem ipsum`. Substitua-os antes de entregar seu relatório.
