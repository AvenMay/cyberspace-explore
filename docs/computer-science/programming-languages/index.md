# Programming Language Explore

## Books

### Coding Standards

- [代码大全 2nd PDF]({{ files_server }}/computer-science/programming-languages/current/代码大全%202ND.pdf)
- [代码整洁之道 EPUB]({{ files_server }}/computer-science/programming-languages/current/代码整洁之道.epub)
- [修改代码的艺术 PDF]({{ files_server }}/computer-science/programming-languages/current/修改代码的艺术.pdf)
- [重构与模式 EPUB]({{ files_server }}/computer-science/programming-languages/current/重构与模式.epub)
- [重构-改善既有代码的设计 PDF]({{ files_server }}/computer-science/programming-languages/current/重构-改善既有代码的设计.pdf)

### Desgin Patterns

- [大话设计模式 EPUB]({{ files_server }}/computer-science/programming-languages/current/大话设计模式.epub)
- [设计模式-可复用面向对象软件的基础 PDF]({{ files_server }}/computer-science/programming-languages/current/设计模式-可复用面向对象软件的基础.pdf)

### Programming Theory

- [计算机程序的构造和解释 2nd PDF]({{ files_server }}/computer-science/programming-languages/current/计算机程序的构造和解释%202ND.pdf)
- [面向对象分析与设计 PDF]({{ files_server }}/computer-science/programming-languages/current/面向对象分析与设计.pdf)

## Projects

- [Awesome Cheatsheets](https://github.com/skywind3000/awesome-cheatsheets)

## Practicality Classification

### Dynamic Language

- 例如：Python、JavaScript
- 优势：快速开发，灵活，生态丰富，适合原型、数据处理、Web开发等。
- 局限：无法直接操作底层硬件或构建操作系统、驱动、嵌入式系统。性能相对低，不能胜任高性能基础设施或系统级编程。

---

### Static Language

- 例如：Java、Go、C#
- 优势：类型安全，适合构建大规模应用、后端服务、企业系统。
- 局限：开发速度比动态语言慢。不擅长直接控制底层硬件或操作系统。对快速迭代和临时脚本化任务不如动态语言方便。

---

### System Level Language

- 例如：C、C++、Rust
- 优势：精确控制内存、CPU、硬件，构建操作系统、驱动、嵌入式系统。高性能，适合对效率要求极高的应用。
- 局限：开发复杂度高，迭代慢，不适合快速交付或原型开发。学习曲线陡峭。

### Functional Language

- 例如：Haskell、OCaml、Erlang
- 优势：函数为一等公民、不可变数据、易并发和数学建模；学术研究、编译器开发、金融建模；科学计算、编译器；高并发分布式系统；数据处理、DSL、Web后台
- 局限：函数式语言优势突出于抽象、安全和并发，但局限在性能开销大、学习曲线陡峭、调试复杂及与现有生态集成困难。

### Core Conclusions

每类语言都有其必然性，无法完全替代：

- Python/Java → 快速开发，但不能做基础设施或系统级任务，换句话说就是应用层语言。
- C/C++ → 高性能基础设施，但迭代慢，不适合快速开发。
