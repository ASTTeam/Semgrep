# 《深入理解Semgrep》

本项目收集整理Semgrep相关内容，包括Semgrep的设计原理实现方法或使用Semgrep进行的漏洞挖掘案例等。Semgrep基于语义的代码分析思想在SAST领域将会是一把利剑，无需编译快速扫描更是其优点。作者：[0e0w](https://github.com/0e0w)

本项目创建于2022年3月17日，最近的一次更新时间为2022年3月20日。

- [01-Semgrep资源](https://github.com/ASTTeam/Semgrep#01-Semgrep%E8%B5%84%E6%BA%90)
- [02-Semgrep基础](https://github.com/ASTTeam/Semgrep#02-Semgrep%E5%9F%BA%E7%A1%80)
- [03-Semgrep语言](https://github.com/ASTTeam/Semgrep#03-Semgrep%E8%AF%AD%E8%A8%80)
- [04-Semgrep进阶](https://github.com/ASTTeam/Semgrep#04-Semgrep%E8%BF%9B%E9%98%B6)
- [05-Semgrep案例](https://github.com/ASTTeam/Semgrep#05-Semgrep%E6%A1%88%E4%BE%8B)
- [06-Semgrep参考](https://github.com/ASTTeam/Semgrep#06-Semgrep%E5%8F%82%E8%80%83)

## 01-Semgrep资源

本章节收集整理Semgrep的相关资源内容，文章内容质量参差不齐，建议深入学习官方资源！

一、官方资源
- [ ] https://semgrep.dev/docs
- [ ] https://semgrep.dev/learn
- [ ] https://github.com/returntocorp/semgrep
- [ ] https://github.com/returntocorp/semgrep-rules
- [ ] https://github.com/returntocorp/semgrep-docs
- [ ] https://github.com/returntocorp/semgrep-action

二、优秀资源
- [x] [《深入理解Semgrep》](https://github.com/ASTTeam/Semgrep)@0e0w
- [ ] https://github.com/tuannq2299/semgrep-rules

三、视频资源

四、学术刊物

五、其他资源
- [x] https://xz.aliyun.com/t/9531
- [x] https://www.anquanke.com/post/id/240028
- [ ] https://zhuanlan.zhihu.com/p/377651159
- [ ] https://zhuanlan.zhihu.com/p/387246394
- [ ] https://www.freebuf.com/articles/web/286643.html
- [ ] https://github.com/trailofbits/semgrep-rules
- [ ] https://github.com/returntocorp/ocaml-tree-sitter-semgrep
- [ ] https://github.com/returntocorp/semgrep-vscode
- [ ] https://github.com/frappe/semgrep-rules
- [ ] https://github.com/semgrep/rules-owasp-asvs
- [ ] https://github.com/jtmelton/semgrep-idea-plugin
- [ ] https://github.com/dgryski/semgrep-go
- [ ] https://github.com/vmnguyen/semgrep-rules
- [ ] https://github.com/returntocorp/semgrepl
- [ ] https://github.com/returntocorp/semgrep-c-sharp
- [ ] https://github.com/returntocorp/semgrep-grammars
- [ ] https://github.com/srijan-deepsource/django-antipatterns
- [ ] https://github.com/quasilyte/go-ruleguard
- [ ] https://github.com/returntocorp/semgrep-rust
- [ ] https://github.com/returntocorp/semgrep-rules-test-action
- [ ] https://github.com/returntocorp/semgrep.vim
- [ ] https://github.com/kondukto-io/semgrep-rules
- [ ] https://github.com/semgrep/template-rules
- [ ] https://github.com/returntocorp/semgrep-ocaml
- [ ] https://github.com/Ayrx/semgrep_introduction
- [ ] https://github.com/g-wilson/action-semgrep
- [ ] https://github.com/ajinabraham/libsast
- [ ] https://github.com/brentjanderson/asdf-semgrep
- [ ] https://github.com/returntocorp/semgrep-hack
- [ ] https://github.com/ligurio/semgrep-rules
- [ ] https://github.com/agigleux-limited/semgrep-evaluation
- [ ] https://github.com/jrgventura7/SemgrepDemo
- [ ] https://github.com/imfht/my-semgrep-rules
- [ ] https://github.com/hsparmar1/semgrep-jdbc-demo
- [ ] https://github.com/minusworld/semgrep-library
- [ ] https://github.com/guyinatuxedo/semgrep
- [ ] https://github.com/dsocastillo/semgreptest
- [ ] https://github.com/returntocorp/semgrep-java
- [ ] https://github.com/majidmc2/SecSnake
- [ ] https://github.com/returntocorp/semgrep-go
- [ ] https://github.com/wahyuhadi/semgrep-integrator
- [ ] https://github.com/0xdea/semgrep-rules
- [ ] https://github.com/pingvin1341/semgrep-pipeline
- [ ] https://github.com/gabrielg/codeclimate-semgrep
- [ ] https://github.com/devidwfreitas/intro-to-semgrep
- [ ] https://github.com/allwin101/intro-to-semgrep
- [ ] https://github.com/007divyachawla/intro-to-semgrep
- [ ] https://github.com/MarceloSFlori/intro-to-semgrep
- [ ] https://github.com/tezamukkavilli-cpi/intro-to-semgrep
- [ ] https://github.com/ymmatheus/intro-to-semgrep
- [ ] https://github.com/phani-gadupudi/intro-to-semgrep
- [ ] https://github.com/hsparmar1/semgrep-java-owasp

## 02-Semgrep基础

 本章节介绍Semgrep的基础用法及设计思路实现原理等！

一、Semgrep安装

二、Semgrep使用
## 03-Semgrep规则

本章节介绍QL语言的语法规则，包括优秀规则等内容。

一、基础语法

二、规则编写
- Java
- C#
- Go

三、官方规则

四、优秀规则
## 04-Semgrep进阶

本章节是针对不同的开发语言进行Semgrep扫描的例子，本章节待整理。

一、Java安全分析

二、C#安全分析

三、Golang安全分析

四、Python

五、C++安全分析

六、Ruby

七、Semgrep工具
## 05-Semgrep案例

本章节介绍Semgrep的具体使用案例，包括自己通过Semgrep挖掘的漏洞等内容。

一、大型应用分析
- 分析Shiro
  - https://www.freebuf.com/articles/web/321757.html
- 分析Fastjson
- 分析Log4j
- 分析Dubbo
- 分析kylin
- 分析grafana
- 分析Hadoop
- 分析Struts2

二、代码审计案例
## 06-Semgrep参考

- https://github.com/ASTTeam/Semgrep

## Stargazers

[![Stargazers @ASTTeam/Semgrep](https://reporoster.com/stars/ASTTeam/Semgrep)](https://github.com/ASTTeam/Semgrep/stargazers)

## Forkers

[![Forkers @ASTTeam/Semgrep](https://reporoster.com/forks/ASTTeam/Semgrep)](https://github.com/ASTTeam/Semgrep/network/members)



![Stargazers over time](https://starchart.cc/ASTTeam/Semgrep.svg)