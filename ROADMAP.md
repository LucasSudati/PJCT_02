# Roadmap — WaveLab

Laboratório de sinais e sistemas. As etapas são incrementais e devem preservar os módulos existentes.

## P0 — Fundação
- [x] DFT educativa, forma de onda, amostragem e áudio (index.html).
- [x] Transformada Z: plano Z, resposta impulsiva e estabilidade (z.html).
- [ ] Testes automatizados para transformadas e filtros.
- [ ] Publicação GitHub Pages e validação mobile.

## P1 — Processamento digital
- [x] FFT radix-2 com 256–2048 pontos e visualização de espectro; benchmark/comparação direta ainda pendentes.
- [x] Filtro FIR de média móvel aplicado ao sinal, com comparação temporal e espectral; resposta ao impulso dedicada pendente.
- [ ] Filtros IIR: passa-baixas e passa-altas, coeficientes e estabilidade.
- [ ] Convolução animada e equações associadas.

## P2 — Sistemas e transformadas
- [ ] Editor de polos e zeros arrastáveis no plano Z.
- [ ] Transformada de Laplace: plano S, região de convergência, polos e zeros.
- [ ] Circuitos RLC: resposta temporal e em frequência.
- [ ] Painel lado a lado Fourier, Z e Laplace.

## P3 — Instrumentação
- [ ] Osciloscópio por microfone, com autorização explícita.
- [ ] Espectrograma e analisador de áudio em tempo real.
- [ ] Simulação ADC: quantização, resolução em bits e erro.

## P4 — Avançado
- [ ] Geradores AM, FM, ASK, FSK e PSK.
- [ ] Ruído controlado, relação sinal-ruído e filtragem.
- [ ] Estimativa de função de transferência a partir de entrada e saída.
- [ ] Exportação de dados e figuras.

## Critérios gerais
- Fórmulas e unidades visíveis; gráficos responsivos; sem dependências quando possível.
- Distinguir simulações educativas de ferramentas de engenharia validadas.
- Manter README conciso e registrar trabalho futuro neste ROADMAP.
