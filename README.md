# Piano_Pure-Data
## Descrição
Este é um projeto de piano virtual desenvolvido no Pure Data (Pd) que contém todas as teclas musicais (C, D, E, F, G, A, B, C1, C#, D#, F#, G#, A#). Além disso, possui um slider que permite o controle do volume do piano.

O objetivo final é exportar esse projeto para o MobMuPlat, permitindo que o usuário possa interagir com o piano virtual através de uma interface gráfica em seu dispositivo móvel.

# Conteúdo
## Objetos
`receive fromGUI`: Receber mensagens do GUI (Interface Gráfica do Usuário)

`list trim`: Remove os espaços em branco da lista recebida

`route`: Recebe uma mensagem e a encaminha para a saída correspondente

`unpack 0 1`: Desempacota uma lista recebida

`select 0`: Seleciona apenas o primeiro elemento da lista

`*~`: Multiplica sinais de áudio

`+ 60`: Adiciona 60 ao valor recebido (Para corresponder a um pitch MIDI)

`+`: Objeto para soma

`mtof`: Converte valor MIDI em frequência

`osc~`: Oscilador de áudio

`*~`: Multiplica os sinais de áudio

`dac~`: saída de áudio

`delay 120`: Atraso de 120ms ao sinal de áudio

`line~`: Curva de rampa linear (Permite transições suaves e graduais entre valores)

## Mensagens
`1 10`: Mensagem para definir a taxa de ataque (Rapidez com que o som atinge seu volume máximo após ser acionado)

`0 500`: Tempo das notas

## Sliders
`vslider`: Slider vertical de volume
