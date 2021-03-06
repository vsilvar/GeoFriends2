# GeoFriends2
An OpenAI Gym environment with complex puzzle maps, highly adequate for reinforcement learning approaches, based on [Geometry Friends](http://gaips.inesc-id.pt/geometryfriends/).

To ready the environment, we recommend using VirtualEnv. You will need the [PyGame](https://www.pygame.org/news) and [Gym](https://github.com/openai/gym) environments.

    python3 -m venv venv
    source venv/bin/activate
    pip install --upgrade pip
    pip install pygame gym
    python TestEnv.py

We also included some deep reinforcement learning examples, using Asynchronous Advantage Actor-Critic and Asynchronous 1-step and n-step Q-Learning. For those, you will need [TensorFlow 1.1+](https://www.tensorflow.org/), and [SciPy](https://www.scipy.org/). You can run both algorithms locally with
  
    export PYTHONPATH=$(pwd)
    python A3C/A3C-LocalThreads.py
    python DQN/DQN-LocalThreads.py

Or distributed with the scripts (for example, 12 processes):

    ./start-a3c.sh 12
    ./start-dqn.sh 12

We are in the process of publishing a paper with more details and our results. We will post those here in the future.
