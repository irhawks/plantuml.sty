# plantuml.sty
latex (xelatex) options to process plantuml code

添加该plantuml.sty可以在latex当中插入plantuml代码，示例如下：

```latex
\begin{plantuml}[width=0.4\textwidth]
@startuml
skinparam dpi 300
class 构件
构件 "1" --> "1..N" 服务
构件 "1" --> "1..N" 接口
接口 "1" -> "1" 服务 : ?
@enduml
\end{plantuml}
```

目前plantuml还不能像includegraphics那样自由设置参数，而且DPI还必须由用户显式设定。
