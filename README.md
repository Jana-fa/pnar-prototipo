# PNAR — telas em teste

Telas do pré-natal de alto risco (PNAR) do MEJC — hospital universitário
UFRN/EBSERH — publicadas para avaliação da equipe em
**https://jana-fa.github.io/pnar-prototipo/**

| Tela | Link |
|---|---|
| 1ª consulta médica | https://jana-fa.github.io/pnar-prototipo/1a-consulta-medica.html |
| Consulta de anestesiologia | https://jana-fa.github.io/pnar-prototipo/anestesiologia.html |

## Antes de usar

- **As telas gravam de verdade.** "Finalizar consulta" envia o atendimento ao
  banco do projeto, e o popup diz o que aconteceu: gravada, não gravada (com o
  motivo) ou gravação não confirmada. **Use apenas dados fictícios**, com
  prontuário começando por `__TESTE_EQUIPE`, enquanto a avaliação estiver em
  curso. Nunca dados de paciente real.
- **Gravada, a consulta fecha.** A tela fica só leitura, com uma faixa que mostra
  a paciente e o protocolo. Para atender outra, use **"Nova paciente"** — ela
  começa do zero e pergunta antes se algo ainda não foi gravado ou exportado.
- **"Exportar atendimento"** gera o texto do que foi preenchido para colar na
  folha de evolução do AGHU; campo em branco não aparece no texto. Fica no popup
  depois de finalizar e na faixa da consulta gravada.
- **Cópia neste navegador.** Cada consulta finalizada também fica guardada no
  navegador de quem preencheu. "Salvar rascunho" grava ali, mas a tela ainda não
  recupera o rascunho. Em computador compartilhado, leve isso em conta.
- O **fullPIERS calcula** quando todos os sete insumos estão preenchidos — falta
  de insumo não vira zero. O número ainda difere da calculadora oficial do
  PRE-EMPT em parte das combinações, e a correção está em decisão: trate-o como
  demonstração.
- Em **Gestação atual**, a DPP e a idade gestacional são calculadas a partir da
  DUM. A IG é editável: corrigida por ultrassonografia, ela é gravada como
  *informada*, e a tela avisa quando difere do cálculo pela DUM.

## Estes arquivos não se editam aqui

`index.html`, `1a-consulta-medica.html` e `anestesiologia.html` são **gerados**
por `scripts/gerar_pagina_publica.py`, a partir das telas que vivem no
repositório de trabalho. Editar uma página aqui não tem efeito: a próxima
geração sobrescreve.

Este repositório existe só para hospedar as páginas no GitHub Pages. O estudo
das variáveis, o registro de decisões e o contrato de backend ficam no
repositório privado do projeto.
