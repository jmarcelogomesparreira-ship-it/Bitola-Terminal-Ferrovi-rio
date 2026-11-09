# Bitola · Terminal Ferroviário

Sala de controle de um terminal rodoferroviário de açúcar VHP: recebimento por caminhão, armazenagem e carregamento de trens. Você opera o terminal, provoca ocorrências e testa cenários, e tudo reage ao vivo.

> Projeto de portfólio com **dados fictícios**, criado por Marcelo José Gomes Parreira.

## Telas

**Operação**
- **Sala de Controle**: gêmeo digital 3D em tela cheia com painéis por cima. Caminhões chegam, pesam e descarregam; a correia leva o açúcar à torre e os vagões enchem um a um. Clique em qualquer equipamento para ver dados e agir sobre ele.
- **Sinóptico**: supervisório no estilo SCADA, com fluxos animados (verde = operando, vermelho = falha), equipamentos clicáveis e tabela de alarmes.

**Análise**
- **Indicadores**: resumo do turno com anel de meta, status dos equipamentos, KPIs, embarque programado × realizado e alertas.
- **Recebimento**, **Trens**, **Armazém**, **Gestão e Custos**, **Pessoas e Segurança**.

**Planejamento**
- **Simulador "E se"**: sliders de moegas, tempo de descarga, chegada de caminhões, taxa da torre, vagões, intervalo entre trens e paradas. Calcula fila (teoria de filas, Erlang C), estadia, capacidade, custo por tonelada e aponta o gargalo. O cenário pode ser aplicado na simulação ao vivo.

## Interatividade

- **Console de operação**: liga/desliga moegas e torre, ajusta a taxa da torre e o ritmo de chegada, chama o próximo trem.
- **Ocorrências simuláveis**: falha na correia, chuva (com chuva no 3D), falta de vagão, falha na balança e pico de caminhões. O impacto aparece nos indicadores e no Pareto de paradas.
- **Detalhamento**: clique em KPIs, barras de gráfico, linhas de tabela, vagões e equipamentos para abrir o detalhe.
- Velocidade **1× / 60× / 300×**, **Modo TV** (Esc para sair), tema claro e escuro, funciona no celular.

## Publicar no GitHub Pages

1. Crie um repositório (ex.: `terminal-ferroviario`) e envie `index.html` e `README.md` para a raiz.
2. Em **Settings → Pages**, escolha a branch `main` e a pasta `/ (root)`.
3. O painel fica em `https://SEU-USUARIO.github.io/terminal-ferroviario/`.

## Tecnologias

HTML, CSS e JavaScript em um único arquivo · [Chart.js](https://www.chartjs.org/) · [Three.js](https://threejs.org/)
