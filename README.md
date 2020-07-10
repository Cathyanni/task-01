task-01
======

# 选择题
* 1  C
* 2  D

# 简答题
* 触发prepatch钩子函数
* 触发update钩子函数
* 对于新节点有text属性，且不等于旧节点text属性的情况
  * 如果老节点有children 则移除老节点children对应的dom元素
  * 设置新节点对应DOM元素得textContent
* 新老节点都有children,且不相等
  * 调用updateChildren()
  * 对比子节点，并且更新子节点的差异
* 只有新节点有children 属性
  * 如果老节点有text属性， 则清空对应DOM元素得textContent
  * 添加所有子节点
* 只有老节点有children属性 移除所有老节点
* 只有老节点有text属性 清空对应DOM元素的textContent
* 触发postpatch钩子函数
