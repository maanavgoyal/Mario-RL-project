# Mario-RL-project
This is a RL agent based on Doubel Deep Q Network algorithms built to play super mario bros.
# Setup
The program uses openai gym and nes python emulator to play the game.
# Preprocessing
To make the AI learn more effeciently we preprocess the data given to it. We reduce the number of possible action space available to the AI to basic 7 simple movement controls instead of all possible key combinations. We convert our RGB frames to greyscale and also normalise the pixel values from 0 to 1 to improve the learning performance of the AI. As every consecutive frame may not be needed for effecient learning our algorithm only returns every 4th frame.
# Learning Algorithm
The AI uses Double Deep Q network. It uses the Bellman equations and Q-update rules to perform remember, recall and experience_replay functions. We also maintain two tables dq1 and dq2 for Double Q learning.
# Results
The OpenAi gym offers several versions of Mario for us to use. Here we compare the learning rate for v0 and v3. Super_mario_bros_v0 is the standard mario whereas the v3 is the rectangular pixelated version.
![image](https://user-images.githubusercontent.com/102295389/178151718-8d2797a5-1179-498a-8cb3-cd08c353ac5d.png)
![image](https://user-images.githubusercontent.com/102295389/178151760-600602e8-309c-4237-b883-bfdc578ba641.png)
