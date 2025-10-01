# MultiAgent
多智能体学习笔记

[**CRAFT: Coaching Reinforcement Learning Autonomously using Foundation Models for Multi-Robot Coordination Tasks**](https://www.alphaxiv.org/abs/2509.14380)

* 大语言模型 (LLMs) 和视觉语言模型 (VLMs) 作为自动化教练，教会多机器人系统完成复杂的协作任务
* 利用LLM将复杂目标分解为子任务，用LLM生成奖励函数
* VLM闭环：
  * 评估：观察机器人执行任务的情况
  * 反馈：若失败会分析原因（奖励函数的学习曲线），生成建议
  * 优化：LLM接受建议并修改奖励函数
* 序贯训练：前一个子任务训练好的策略权重会用作下一个更难子任务的初始权重



