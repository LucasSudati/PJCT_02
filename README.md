# WaveLab

Laboratório interativo de sinais e amostragem, desenvolvido em HTML, CSS e JavaScript puro.

## Módulos

- **Fourier (DFT):** [abrir laboratório de sinais](./index.html) — análise espectral já implementada em JavaScript.
- **Transformada Z:** [abrir laboratório de sistemas digitais](./z.html) — plano Z, polo/zero, estabilidade e respostas de um filtro causal de primeira ordem.
- **Laplace (planejado):** adicionar plano S, polos e zeros, região de convergência e respostas de sistemas contínuos, incluindo exemplos RLC. Ainda não implementado.

## Funcionalidades

- Geração de ondas senoidais, quadradas, triangulares e dente de serra.
- Controle de frequência, amplitude e fase.
- Ajuste da taxa de amostragem e visualização das amostras sobre o sinal.
- Espectro de frequências calculado por transformada discreta de Fourier (DFT) de 256 pontos.
- Indicadores de frequência de Nyquist, amostras por ciclo e período.
- Avisos educativos sobre aliasing.
- Reprodução de áudio pelo navegador com Web Audio API.
- Interface responsiva, sem dependências externas.

## Executar

Abra o arquivo `index.html` (Fourier) ou `z.html` (Transformada Z) em um navegador moderno. Não é necessário instalar pacotes ou iniciar um servidor.

Também é possível publicar o projeto no GitHub Pages selecionando a branch `main` e a pasta `/ (root)` em **Settings → Pages**.

## Como experimentar

Selecione uma onda senoidal com frequência de 12 Hz e taxa de amostragem de 80 Hz. Depois, aumente a frequência para 50 Hz e observe a mudança das amostras e o aviso de Nyquist. Experimente também ondas quadradas para comparar seus harmônicos no espectro.

## Notas técnicas

O gráfico temporal mostra uma janela de 250 ms. O espectro aplica uma DFT diretamente às 256 amostras e exibe frequências entre 0 e a frequência de Nyquist. Não há janela espectral adicional; vazamento espectral pode ocorrer. A reprodução sonora multiplica a frequência visual por 20 para tornar o sinal audível, preservando a forma da onda. A fase configurada afeta a visualização e a DFT, mas não o oscilador sonoro. A verificação de Nyquist se refere à fundamental; ondas com harmônicos podem apresentar aliasing abaixo desse limiar.

## Licença

Código disponibilizado para fins de estudo e experimentação.
