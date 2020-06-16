Experience Replay Optimization
Daochen Zha , Kwei-Herng Lai , Kaixiong Zhou and Xia Hu

•	https://arxiv.org/abs/1906.08387

•	Novel experience replay optimization (ERO) framework

o	alternately updates two policies: the agent policy, and the replay policy

o	The agent is updated to maximize the cumulative reward based on the replayed data, while the replay policy is updated to provide the agent with the most useful experiences.

•	the uniform sampling cannot reflect the different importance of past experiences: the agent can usually learn more efficiently from some experiences than from others

•	prioritize important experiences

o	directly prioritize the transitions1 with higher temporal difference (TD) errors

o	indirectly prioritize experiences through managing the replay memory

•	the rule-based replay strategies may be sub-optimal and may not be able to adapt to different tasks or reinforcement learning algorithms

•	use of the environmental feedback to update the replay policy

•	ERO enhanced DDPG

•	Update Replay Policy


•	ERO VS PER-prop VS PER-rank VS Vanilla-DDPG

•	the replay policy of ERO is updated to replay the most suitable transitions during training

•	exploiting the improvement of the policy as a reward to update the replay policy is promising

•	rule-based prioritized replay strategies do not provide clear benefits to DDPG on the 8 continuous control tasks

•	ERO requires slightly more running time than Vanilla-DDPG

•	the replay policy provides past experiences to the agent for training

