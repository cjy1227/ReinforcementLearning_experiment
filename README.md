# ReinforcementLearning_experiment
最近在做一些强化学习方面的工作，这里对一些传统的强化学习算法做一个总结，不断整理。
本repo提供的代码，参考莫烦和baseline进行实现，实验环境基于openai gym, 不涉及图像处理相关，较为纯净的强化学习部分实现。
实验结果主要以gym的实验结果为主，有一些实验是在自己实现的一套1v1 6DoF飞行器博弈仿真环境做的实验，该环境较为复杂，对各种算法也有更加全面的验证。

## DQN系列
已完成：     
1. [Nature DQN](http://www.nature.com/articles/nature14236)      
2. [Double DQN](https://arxiv.org/abs/1509.06461)     
3. [Dueling DDQN](https://arxiv.org/abs/1511.06581)    
4. [DRQN](https://arxiv.org/abs/1507.06527)    
5. [Multistep DQN](https://arxiv.org/abs/1703.01327)           

[DQN_IN_PROJECT](https://github.com/zhkmxx9302013/ReinforcementLearning_experiment/tree/master/DQN_IN_PROJECT)目录为整理成项目架构形式的算法，可以兼容以上五种算法，将网络结构，agent学习，主程序分开封装。      

三类算法对比：(DQN, DoubleDQN, Dueling DQN)
1. gym CartPole-v0 环境：
![x](https://res.cloudinary.com/djhkiiiap/image/upload/v1548387003/%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20190125112753.png)
2. 1v1 6DoF飞行器博弈仿真环境做的实验(mean_reward越大越优)
![x](https://res.cloudinary.com/djhkiiiap/image/upload/v1548492902/%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20190126165446.png)


## @Todo
- [x] DRQN 考虑加入部分可观马尔科夫时序处理
- [x] Multistep DQN
- [ ] Priority Replay buffer
