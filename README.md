# Condicionamento de Sinais em Ecoacústica: Filtros RC Analógicos e Digitais
---

Este repositório contém os códigos-fonte desenvolvidos para o projeto final da disciplina de T10199 - Circuitos Elétricos. O objetivo principal é aplicar conceitos fundamentais de redes passivas de primeira ordem (filtros passa-baixas e passa-altas RC) no pré-processamento de dados de ecoacústica, visando atenuar ruídos abióticos e antropogênicos de gravações ambientais.

Os scripts foram estruturados em Python (ambiente Jupyter Notebook) e atuam em três frentes principais de processamento digital de sinais (PDS):

* **Análise Tempo-Frequência:** Cálculo da Transformada de Fourier de Tempo Curto (STFT) e plotagem de espectrogramas em escala logarítmica (dB) para a visualização da densidade espectral dos áudios brutos e filtrados.
* **Simulação de Hardware (IIR):** Implementação de filtros digitais do tipo *Infinite Impulse Response* (Butterworth, 1ª ordem) calibrados para emular matematicamente o exato decaimento e frequência de corte das montagens físicas em protoboard.
* **Aquisição Analógica-Digital:** Rotinas para a captação em tempo real e normalização de ganho do áudio condicionado pelo circuito elétrico físico, lido através da porta de microfone do computador.

## Tecnologias e Bibliotecas Utilizadas
* `librosa` e `soundfile` para manipulação de áudio e extração de características acústicas.
* `scipy.signal` para a modelagem matemática e aplicação dos filtros digitais.
* `sounddevice` para interfaceamento direto com o hardware de gravação (placa de som).
* `matplotlib` para a renderização gráfica comparativa dos resultados.
