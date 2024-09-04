<h1 align="center">
  <img src="https://user-images.githubusercontent.com/40550247/72228004-81071600-3581-11ea-9972-1cbe906001ed.png" width="120px" />
</h1>

<h1 align="center">
   
AI - Pingpong 
</h1>
### Prerequisites
* Python (>= 3.6)

## Getting Started
1. Fork este repositório e clone em sua máquina
2. Mude o diretório para `pingpong-IA` onde você o clonou;
3. No terminal, execute:

```bash
/* Install dependencies */

$ pip install -r requeriments.txt

/* Coletar dados */

$ python PingPongCollect.py

/* Treinar dados */

$ python NeuralNetwork.py

/* Executar IA */

$ python PingPongIA.py
```

### Neural Network
A rede neural possui: uma camada de entrada de 2 neurônios, uma camada oculta de 30 neurônios e uma camada de saída de 1 neurônio. É possível personalizar a quantidade de neurônios de cada uma das camadas.


## File Structure

```bash
pingpong-IA
├── src/
│   ├── database/
│   │   ├── controller/
│   │   │   └── db.py
│   │   ├── data/
│   │   │   └── data-50.txt
│   │   └── weights/
│   │       ├── weight-w1.txt
│   │       └── weight-w2.txt
│   ├── network/
│   │   └── NeuralNetwork.py
│   ├── PingPongCollect.py
│   └── PingPongIA.py
├── .gitignore
├── LICENSE.md
├── README.md
└── requeriments.txt
```

### Vision
O objetivo desse jogo é fazer com que a palheta impeça a bolinha de tocar no chão. A implementação consiste no aprendizado de máquina supervisionado, portanto, teremos que passar ao jogo dados iniciais para que ele processe o aprendizado. A partir do arquivo ``src/PingPongCollect.py``, será executado o jogo para que você jogue, e sejam coletadas informações que serão usadas no aprendizado de sua máquina, então, os dados serão salvos em ``src/database/data``. Logo em seguida, você poderá treinar seus dados de duas formas. Na primeira forma, você poderá executar os dados coletados diretamente na rede neural sem precisar jogar, nesse caso, no ```terminal```, será impressa uma informação, que é a taxa de error do treinamento de sua rede neural, quanto menor a taxa, melhor, após isso, no final deste treinamento, serão salvos os pesos em ```src/database/weights``` (esses pesos são as informações dos neurônios treinados na sua rede neural, ou seja, eles funcionam como um cérebro com o conhecimento em si). Na segunda forma, você irá treinar a sua rede diretamente jogando, no caso, enquanto se joga, a rede treina. Para fazer a sua máquina jogar, você terá que executar o arquivo ```src/PingPongIA.py```. Nele, ou você seta os pesos emitidos pelo treinamento de sua rede ou não passar nenhum peso e deixar o aprendizado começar do zero.

<h1 align="center">
  <img src="https://user-images.githubusercontent.com/40550247/72691686-149e9080-3b06-11ea-863f-10a38f5f6e60.gif"/>
</h1>
---
