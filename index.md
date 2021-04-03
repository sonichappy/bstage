# 1. elasticsearch介绍

## 1.1. 分布式检索引擎

### 1.1.1. 特点
* `基于Apache Lucene引擎`

* `RESTful风格`

* `replica、shards`

* `多租户`

* `无需预定义模式（schema)`

### 1.1.2. index、doc、mapping

|类型|说明|
|---|---|
|index|相当于一个数据库，存储所有的文档；每个ES集群可以创建多个index|
|doc|文档本身，包括多个属性|
|mapping|数据结构描述，一个index对应一个mapping|

* `ES 7.X之前，还有一个Type的概念，介于index和doc之间，相当于RDBMS中的表概念，mapping是和Type绑定的。ES 7.X之后取消了Type概念，每个index只能绑定一种mapping，简化了概念。`
* `在网上检索elasticsearch文档的时候尽量看官网并选对版本，避免不兼容。`


## 1.2. 倒排索引

```flow
st=>start: 开始框
op=>operation: 处理框
cond=>condition: 判断框(是或否?)
sub1=>subroutine: 子流程
io=>inputoutput: 输入输出框
e=>end: 结束框
st->op->cond
cond(yes)->io->e
cond(no)->sub1(right)->op
```

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## 1.3. Commandssss

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## 1.4. Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

```

```