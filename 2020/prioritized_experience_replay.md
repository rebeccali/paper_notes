# Prioritized Experience Replay 
## Tom Schaul, John Quan, Ioannis Antonoglou, David Silver
* https://arxiv.org/abs/1511.05952
* Stochastically prioritize by high TD error (how surprising) samples
* Binary Heap data structure for priority
* Use importance sampling to carefully reweight the gradient update
* Trains DQN and DDQN faster
* Motivating example: Cliff walk (sparse reward, exploration problem, highly redundant failure cases)
* May need to recompute TD-error of previous samples with Value function model
* Implementation notes: Clipped TD-error and rewards to $$[-1, 1]$$
* Thoughts: should clustered experiences have similar TD-error, and something with abnormal TD-error mean it is in a different cluster or the cluster just needs to be updated?
* Replay Frequency is a good metric for how "useful" a sample is, or also for where to explore/whether to keep sample in the buffer
