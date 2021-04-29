# OpenSourceMonitor
Use Telegraf, Prometheus, Grafana to Monitor Server Network and ITO devices
[Link of Course]!(https://mp.weixin.qq.com/s?__biz=MzU5MzUxMDkyNQ==&mid=2247484727&idx=1&sn=a3803e5e4fbde8501e6f0095daa2376f&chksm=fe0e1255c9799b434b3a1f20dbdc9832830ca4b51d5cf809aff34786ef9aace955db98b96652&token=894612663&lang=zh_CN#rd)

Telegraf是我们整个TGP的数据采集部分。因为后面接的是Prometheus，所以Telegraf充当了Metric exporter的功能，得益于Telegraf强大的插件架构，可以实现各式各样的数据采集模式（不管是作为client端，还是server端），然后输出到后端的数据存储（这里的Prometheus)



### github code
https://github.com/udemy-course/telegraf-prometheus-grafana/tree/v0.2


### SNMP of telegraf
https://github.com/xiaopeng163/docker-compose-tpg


## Prometheus

在cloud native（云原生）的领域，Prometheus是非常著名的，它是继kubernetes之后第二个加入云原生云计算基金会（CNCF）的托管项目。在容器时代，Prometheus几乎可以说是监控Monitoring和报警Alerting toolkit 的标配

•官方网站：https://prometheus.io
•源代码：https://github.com/prometheus

features：
* Time series data model
* PromQL, a flexible query language
* time series collection happens via a pull model over HTTP

[![Architecture](https://prometheus.io/assets/architecture.png)](https://prometheus.io/docs/introduction/overview/#architecture)


components:
* scrapes and stores time series data
* client libraries for instrumenting application code
* a push gatew way for supporting short-live jobs
* special-purpose exporters for services like HAProxy, StatsD, Graphite, etc
* an alertmanager to handle alerts




### Prometheus的内容主要包括：

•架构介绍
•Metric类型介绍
•PromQL的基本查询
•Metric Exporter介绍
•Pushgateway
•Alerting&Rule报警
