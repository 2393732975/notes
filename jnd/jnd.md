## A survey on just noticeable distortion estimation and its applications in video coding


本文的主要贡献可以简要概括如下：首先，系统地回顾了JND概念的一般描述和现有的JND计算模型。其次，介绍了基于jnd的感知图像和视频编码方案的大部分相关工作，包括基于jnd的编码预处理和基于jnd的编解码器嵌入。第三，对JND估计和基于JND的PVC进行了全面的总结，并对未来可能的发展方向和机遇进行了分析和讨论。

现有的基于jnd的感知图像/视频编码方案可分为基于jnd的编码预处理和基于jnd的编解码器嵌入两大类。在基于JND的编码预处理中，根据JND模型对感知冗余进行预估。在感知质量相近的前提下，对原始图像或视频进行基于jnd的滤波平滑处理，去除感知冗余。相反，基于JND的编解码器嵌入将JND估计过程直接引入到图像/视频编码过程中，并通过对不同编码模块的感知优化大大节省了比特率。

第2节和第3节回顾了JND估计和基于JND的感知视频编码。第4节讨论了未来的方向和机会。第五部分最后对本文进行了总结

读到第三节了

### 基于jdn的编码预处理

**背景介绍**
JND (Just Noticeable Difference): 表示人眼刚刚能够感知到的变化阈值。基于JND的预处理可以去除人类视觉系统（HVS）无法感知的冗余信息，从而减少编码数据量。
**预处理目标:**
1. 在编码之前利用JND模型移除感知冗余。
2. 提高压缩效率而不影响主观视觉质量。

根据**应用域**的不同，预处理分为 空间域的JND编码预处理 (Spatial-JND Coding Preprocessing) 和 子带域的JND编码预处理 (Subband-JND Coding Preprocessing)。


**1. 空间域的JND编码预处理 (Spatial-JND Coding Preprocessing)**


