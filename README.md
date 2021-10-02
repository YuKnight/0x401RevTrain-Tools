# ReverseTools

在最近的CTF比赛，以及一些实际场景中，出现了许多光靠人力手动分析和动态调试难以解决的问题，例如用脚本生成的垃圾代码、一些复杂的代码混淆等等。此时我们往往需要借助一些辅助分析工具来帮助我们完成半自动化的逆向分析或代码反混淆，在CTF比赛的某些题目中，我们甚至可以用这些工具在不分析加密算法的情况下直接梭哈得到flag。

本仓库整理了一些逆向辅助分析神器的原理和用法，目前已经整理的内容如下：

**静态分析类：**

- `capstone`：汇编/反汇编框架

**符号执行类：**

- `angr`：应用最广泛的符号执行引擎
- `miasm`：综合了静态分析、符号执行、模拟执行、动态符号执行的集大成逆向框架

**模拟执行类：**

- `unicorn`：基于QEMU的模拟执行引擎

**约束求解类：**

- `z3`：微软开发的约束求解器（通俗一点就是方程/方程组求解器），是angr和miasm的约束求解实现
