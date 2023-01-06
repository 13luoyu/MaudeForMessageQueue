# 《代数形式化方法》课程项目：使用Maude建模消息队列

### 安装

    apt-get install maude
    maude

### 运行不带优先级消息队列的建模

    load state.maude
    load task.maude
    load mq.maude
    load mq_op.maude

    search ic =>* (pc[I:Task]: out) (pc[J:Task]: out) C:Config .
    show path 9 .


### 运行带优先级的消息队列的建模

    load state.maude
    load task.maude
    load ptask.maude
    load pmq.maude
    load pmq_op.maude

    search ic =>* (pc[I:PriorityTask]: out) (pc[J:PriorityTask]: out) C:Config .
    show path 9 .



