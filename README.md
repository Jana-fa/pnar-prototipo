# PNAR — protótipo da 1ª consulta médica

Protótipo de tela para avaliação, publicado em
**https://jana-fa.github.io/pnar-prototipo/**

Pré-natal de alto risco (PNAR) do MEJC — hospital universitário UFRN/EBSERH.

## Antes de usar

- **Nada é gravado.** O formulário roda inteiro no navegador de quem abre;
  fechar a aba apaga o preenchimento. Nenhum dado sai do aparelho.
- **Use apenas dados fictícios.** Não preencha com dados de paciente real.
- O **fullPIERS calcula** quando todos os sete insumos estão preenchidos —
  falta de insumo não vira zero, e a probabilidade ainda está em conferência
  manual contra as calculadoras publicadas. Trate o número como demonstração.
- O botão **"Exportar atendimento"** gera o texto do que foi preenchido para
  colar na folha de evolução; campo em branco não aparece no texto.

## Este arquivo não se edita aqui

`index.html` é **gerado** por `scripts/gerar_pagina_publica.py`, a partir do
protótipo que vive no repositório de trabalho. Editar a página aqui não tem
efeito: a próxima geração sobrescreve.

Este repositório existe só para hospedar a página no GitHub Pages. O estudo das
variáveis, o registro de decisões e o contrato de backend ficam no repositório
privado do projeto.
