# HIT_SoftwareEngineering_Lab1
## 哈尔滨工业大学计算机学院软件工程 Lab1 结对编程
**本次实验共需完成六种需求：**
### √ 文本生成图
```
将文本按题目要求规范化后，以文本中的单词作为结点，按照指定要求建立有向图，用邻接表存储，结点之间的权值为两个单词在文本中相邻的次数（例如，A B相邻n次，则A -> B边上的权值为 n）。
```
### √ 展示有向图
```
根据邻接表中存储的有向图信息，利用GraphViz画出有向图并展示。
```
### √ 查询桥接词（word1，word2）
```
有向图的广度优先搜索的简化版本，只需搜索包含其实结点word1在内的三层结点即可。依次将word1可达的单词结点入队，判断入队的单词结点是否可达word2，若可达，则该单词结点为桥接词；反之，不是。
```
### √ 根据桥接词生成新文本
```
承接上一功能，依次查询相邻两个单词之间的桥接词，若存在，则在两相邻单词之间加入桥接词；否则，不加入，最后，输出新文本。
```
### √ 计算最短路径
```
读取图和出发点之后使用修改过的Dijkstra算法计算最短路径，并在算法寻路中把每个点的前驱父节点存入父节点数组，若有多个则一并存入，之后看输入的词个数，若一个则递归输出所有的路径，两个就输出特定的路径。对Dijkstra算法的改动就是在贪心算法比较路径时，若有相同的长度则一并填入，而不是只寻找小于的情况。对距离排序中使用了优先队列（二叉堆）进行优化。
```
### √ 随机游走
```
开始随机选择一个起始结点，然后随机访问该结点可达的结点，如此进行下去，直到所访问的结点没有出边或走过一条重复的边，或者用户停止，则随机游走停止，将访问路径保存到电脑磁盘。
```
### 程序运行效果图
<div align=center><img width="500" height="300" src="https://github.com/AIRobotZhang/HIT_SoftwareEngineering_Lab1/raw/master/Graphpic.png" alt="有向图G的存储结构"/></div></div>


<div align=center><img width="500" height="300" src="https://github.com/AIRobotZhang/HIT_SoftwareEngineering_Lab1/raw/master/login.png" alt="有向图G的存储结构"/></div></div>


<div align=center><img width="500" height="500" src="https://github.com/AIRobotZhang/HIT_SoftwareEngineering_Lab1/raw/master/firstpage.png" alt="有向图G的存储结构"/></div></div>


<div align=center><img width="500" height="370" src="https://github.com/AIRobotZhang/HIT_SoftwareEngineering_Lab1/raw/master/filechooser.png" alt="有向图G的存储结构"/></div></div>


<div align=center><img width="500" height="500" src="https://github.com/AIRobotZhang/HIT_SoftwareEngineering_Lab1/raw/master/showgraph.png" alt="有向图G的存储结构"/></div></div>


<div align=center><img width="500" height="300" src="https://github.com/AIRobotZhang/HIT_SoftwareEngineering_Lab1/raw/master/calshortestpath.png" alt="有向图G的存储结构"/></div></div>
