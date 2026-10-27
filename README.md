# Conciliador JBC

JBC Micro Sistemas — conciliação de clientes e fornecedores. Monta a composição nota a nota a partir da composição do ano anterior e do razão auxiliar (Mastermaq), confere os totais e aponta o que precisa ser apurado.

Os arquivos são lidos apenas no navegador; nada é enviado a servidor.

Publicado em https://jbccontabil.github.io/conciliador/

## Conciliação de Notas de Débito (`nd.html`)

Segunda ferramenta do repositório: concilia a conta de NDs a receber a partir do razão (Mastermaq, `.xls`) e da lista de NDs emitidas (`.xlsx`). Aponta NDs em aberto, recebimentos sem emissão no período, NDs só na lista, divergências de valor e confere o saldo. Exporta Excel com composição, todas as NDs e conferência.

Publicado em https://jbccontabil.github.io/conciliador/nd.html

## Bibliotecas

As duas bibliotecas de planilha ficam em `vendor/`, servidas pelo próprio repositório (sem CDN):

- `xlsx.full.min.js` — SheetJS 0.18.5 (Apache-2.0), leitura de `.xls`/`.xlsx`
- `exceljs.min.js` — ExcelJS 4.4.0 (MIT), geração do Excel formatado
