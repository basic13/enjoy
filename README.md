### Enjoy

Enjoy 是基于 Java 语言的极轻量极魔板引擎。极轻量级仅 171K 并且不依赖任何第三方。极简设计仅 if、for、set、define、include、render 六个核心指令，让学习成本低到极致。独创 DKFF(Dynamic Key Feature Forward) 词法分析算法与 DLRD (Double Layer Recursive Descent)语法分析算法，避免使用 javacc、antlr、jflex 生成器，令代码量少到极致。

#### Enjoy 主要特点
- 消灭传统模板引擎中大量繁杂概念，仅六个核心指令，学习成本极低
- 独创 DKFF 词法分析算法与 DLRD 语法分析算法，避免使用javacc、antlr
- 功能强大，极为简单覆盖掉 freemarker、velocity 的核心功能
- 扩展性强，支持多种扩展方式，且是唯一支持指令级扩展的模板引擎
- 与 java 打通式设计，在模板中与 java 交互极为方便
- 贴近 java 使用直觉，为 java 开发者量身打造
- 回归模板引擎渲染 View 数据的本质，采用指令式设计，避免 view 层表达复杂逻辑
- 体积小，仅 171K，且不依赖于任何第三方


#### 简单示例：

**1. 在 spring 中的配置**

```java
<bean id="viewResolver" class="com.jfinal.template.ext.spring.JFinalViewResolver">
	<!-- 是否热加载模板文件 -->
	<property name="devMode" value="true" />
	<!-- 配置shared function，多文件用逗号分隔 -->
	<property name="sharedFunction" value="/view/_layout.html, /view/_paginate.html" />
	
	<!-- 是否支持以 #(session.value) 的方式访问 session -->
	<property name="sessionInView" value="true" />
	<property name="prefix" value="/view/" />
	<property name="suffix" value=".html" />
	<property name="order" value="1" />
	<property name="contentType" value="text/html; charset=utf-8" />
</bean>
```

**2.详细使用方法见 jfinal 手册**
read me 正在补充，详细使用文档请下载 jfinal.com 官网的 jfinal 手册[http://www.jfinal.com](http://www.jfinal.com)

**JFinal 官方网站：[http://www.jfinal.com](http://www.jfinal.com)**




