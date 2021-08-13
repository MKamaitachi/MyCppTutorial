# 前言

## 为什么写这本书

受某位提问箱的匿名朋友的建议，我建立了这份文档，用于记录我所希望的一套 C++ 教学方案。**请注意，我只负责讲解 C++ 语法层面的知识。对于超过语法的问题（比如算法设计、计算机系统等）不在本书的讨论范围之内**；书中所引用的算法仅作为例子使用。尽管许多批评家说这是不负责任的行为，但是我认为一份教材应当只做好一件事情。有关算法部分的学习，我建议阅读本书的前五章（第〇章 \~ 第四章）作为 C++ 的基础，然后选用任意一本算法教材进行学习即可。

最初我计划将这些想法纳入尚未成型的北京大学《计算概论（A）》教材中，但是由于指导教师没有（时间或精力）领导团队，我只得暂时将这些想法暂且记录在这里。除此之外，我还将《程序设计实习》中语法部分的内容以及更多的现代 C++ 编程方法以个人讲解的方式一并给出。故总的来说，你将看到如下内容：

- 第〇章：非常简单的基本计算机知识概述；内容属于北京大学《计算概论（A）》“计算机基础知识”部分。
- 第一 \~ 四章：用 C++ 的语法讲述 C 语言知识；教学思路依照北京大学《计算概论（A）》课程，少量穿插新语法特性。其性质属于教材草案。
- 第五 \~ 八章：讲解 C++ 面向对象语法，但以实用为主、思想为辅；大体框架依照北京大学《程序设计实习》课程。其性质属于知识整理。
- 第九 \~ ? 章：讲解一些必要的 C++ 相关知识。
- 第 ? \~ ? 章：讲解 C++ 更深入的语法，包括函数式编程等。其性质属于读书笔记。

尽管我将此项目命名为“谷雨同学的 C++ 教程”，但由于未经任何实践的教学，我并不能考察、估计这份“教程”对初学者所能提供的帮助作用。**相对地，本文更倾向于那些准备或正在接受传统课内学习的学生。**再次提醒，我只是在此循序渐进地描述了 C++ 语法标准的规定；若要想熟练运用 C++ 编写程序，仅仅靠这份文档是完全不够的。只有将教程中所提到的语法和技术投入到实践中去，才能真正掌握这门语言。

为了防止版权问题，此文档未经授权**禁止转载**。

> 我尝试了各大电子书（文档）发布平台，如 GitBook 、看云和语雀等，但是都不甚满意：
> - GitBook 国内连接速度堪忧，且对中文输入支持不好；
> - 看云太丑，免费功能较少，编辑体验不佳；
> - 语雀导入导出功能偏弱，还有待发展；
> 
> 最终选择了 Docsify 工具自行搭建文档的方法。经过长时间的调试目前已经可以很好地阅读了，但仍然可能存在排版错误还请谅解，并希望您能及时指出。

## 联系方式

如果您对书中的内容存在疑问、建议或意见，请通过邮箱 [guyutongxue@163.com](mailto:guyutongxue@163.com) 联系我，谢谢您的支持与配合。

## 一些约定

本文中用“我”来指代作者，用“你”来指代读者；“我们”一词一般用于指明过去或接下来需要做的事情，仅用于补足主语，没有更多意义。本文的一些地方可能用词不是特别严谨，还请各位读者见谅。

本文中“引用的部分”（指灰色底纹的那些，比如——
> 引用

这样的），属于对正文的补充。对于那些有一定基础的读者，这些内容会有助于架构更加完善的知识体系；而没有基础的读者完全可以跳过这些部分。

本书是面向 C++20 标准的（模块除外，因为编译器未能广泛支持）。对于有基础的读者来说，至少请将你的编译器升级到能完整支持 C++11 标准（GC除外）的版本。对于常见的编译器，要求：

- GCC 版本 4.8.1 及以上
- Clang 版本 3.8 及以上
- MSVC （Visual Studio）版本 19.26 及以上

## 其它

> 厚颜无耻地放个码……如果你觉得这本书有帮助或者还不错的话，就打个赏呗。
> 
> <div style="text-align: center">
> <img alt="Alipay QR code" src="assets/alipay.jpg" width="200">
> <img alt="WeChat QR code" src="assets/wechat.jpg" width="200">
> </div>
