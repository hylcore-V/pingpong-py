<h1 align="center">
  <img src="https://user-images.githubusercontent.com/40550247/72228004-81071600-3581-11ea-9972-1cbe906001ed.png" width="120px" />
</h1>

<h1 align="center">
   
AI - Pingpong 
</h1>
### Prerequisites
* Python (>= 3.6)

## Getting Started
1. Fork this repository and clone it to your machine.
2. Change the directory to pingpong-AI where you cloned it.
3. In the terminal, execute:

```bash
/* Install dependencies */

$ pip install -r requeriments.txt

/* Collect data */

$ python PingPongCollect.py

/* Train data */

$ python NeuralNetwork.py

/* Execute AI */

$ python PingPongAI.py
```

### Neural Network
The neural network has: an input layer with 2 neurons, a hidden layer with 30 neurons, and an output layer with 1 neuron. It is possible to customize the number of neurons in each layer.


## File Structure

```bash
pingpong-AI
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
│   └── PingPongAI.py
├── .gitignore
├── LICENSE.md
├── README.md
└── requeriments.txt
```

### Vision
The objective of this game is to prevent the paddle from letting the ball touch the ground. The implementation consists of supervised machine learning, so we will have to provide the game with initial data for it to process the learning. Starting from the file src/PingPongCollect.py, the game will be executed for you to play, and information will be collected that will be used in the learning of your machine; then, the data will be saved in src/database/data. Immediately after, you can train your data in two ways. In the first way, you can execute the collected data directly in the neural network without needing to play; in this case, in the terminal, information will be printed, which is the error rate of your neural network's training—the lower the rate, the better. After this, at the end of this training, the weights will be saved in src/database/weights (these weights are the information of the neurons trained in your neural network, i.e., they function like a brain with the knowledge itself). In the second way, you will train your network directly by playing; in this case, while playing, the network trains. To make your machine play, you will have to execute the file src/PingPongAI.py. In it, you either set the weights emitted by the training of your network or pass no weights and let the learning start from scratch.

<h1 align="center">
  <img src="https://user-images.githubusercontent.com/40550247/72691686-149e9080-3b06-11ea-863f-10a38f5f6e60.gif"/>
</h1>
---
