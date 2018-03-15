1、神经网络激励函数的作用:不使用激励函数的话，神经网络的每层都只是做线性变换，
多层输入叠加后也还是线性变换。因为线性模型的表达能力不够，激励函数可以引入非线性因素。
加入非线性激励函数后，神经网络就有可能学习到平滑的曲线来分割平面，而不是用复杂的线性组合逼近平滑曲线来分割平面。
这就是为什么我们要有非线性的激活函数的原因

2、 To compute the function using a shallow network circuit, you will need a large network
 (where we measure size by the number of logic gates in the network),
 but (ii) To compute it using a deep network circuit, you need only an exponentially smaller network.
 神经网络深度可以用电路理论来解释，如果很浅，每一层都需要用很多节点才能实现

N个输入，o(2^n)

深度神经网络，o(log2(n))

3、如果激励函数为线性函数，再多层也是将输入线性组合，深度没用
   如果初始化W1为0，那么第一层每个节点作用都一样，再多节点也没用