---
sidebar_label: 数字表冠
---

# 数字表冠

数字表冠是手表设备的主要硬件输入。当人们旋转表冠时，它会生成可用于增强或促进与应用程序交互的信息，例如滚动或操作标准或自定义控件。您可以实施的一组方法来跟踪用户与数字表冠的交互，在用户旋转表冠或旋转停止时接收通知。

## 设计原则

- 在滚轮慢速滚动时，页面内容每两个页面刷新间都应该平滑有动画的移动。
- 页面停下时要根据表冠停止滚动前的加速度决定停下后的动画减速曲线。
- 所有页面转动的效果在用户感知层面应该大致相同。
- 整体旋转防误触需要达到的效果：当用户在应用列表有明显旋转意图时需要有响应（明显旋转意图参数定义见下方表格），没有明显旋转意图时页面不应该有抖动。

## 使用规则

**双重防误触逻辑**

**第一层：不表现给用户的防误触**

数字表冠从静止（连续 1 秒没有数值上报）到开始有旋转数值上报：第一次满足连续 20 个周期（每个周期 16ms）均有变化数值上报时，才在页面上表现给用户和数字表冠相关的响应（如：列表旋转、长页面滚动等）

**第二层：表现给用户的防误触**

当旋转通过第一层的筛选，第二层防误触逻辑触发，根据不同的控件类型使用不同的防误触效果，需要有明显旋转意图时才给用户触发页面对应的旋转效果，否不做旋转效果达成的处理。（比如：列表页面旋转式，满足第一层，不满足第二层，在页面看到的效果是反复在此列表项内微微跳动，不会旋转到下个列表项目）。