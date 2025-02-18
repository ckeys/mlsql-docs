# MLSQL 文档

## MLSQL 介绍

* [MLSQL 介绍](README.md)
* [所有版本](release-notes/README.md)
   * [MLSQL Stack版本管理策略](release-notes/version.md)
   * [MLSQL Stack 2.1.0版发布](release-notes/2.1.0.md)
   * [MLSQL Stack 2.0.1版发布](release-notes/2.0.1.md)
   * [MLSQL Stack 2.0.0版发布](release-notes/2.0.0.md)
   * [MLSQL Stack 2.0.1 Bug 合集](release-notes/2.0.1-bug.md)
   * [MLSQL Stack 2.0.0 Bug 合集](release-notes/2.0.0-bug.md)

## 快速启动

* [基本安装](howtouse/README.md)
   * [MLSQL Console 安装](howtouse/install.md)
   * [MLSQL Console 初始配置](howtouse/setup.md)
   * [MLSQL Engine 安装与配置](howtouse/engine/README.md)
       * [启动参数详解](howtouse/engine/configuration.md)
       * [Local](howtouse/engine/deploy.md)
       * [全手工K8s部署](howtouse/engine/k8s_deploy.md)
       * [使用mlsql-deploy部署K8s](howtouse/engine/prebuilt_image_k8s_deploy.md)
       * [Yarn部署](howtouse/engine/yarn_deploy.md)
   * [MLSQL 桌面版安装使用](howtouse/mlsql_desktop_install.md)    
   * [MLSQL 命令行安装与配置](howtouse/mlsql_lang_cli.md)
   * [Sandbox 使用指南](howtouse/sandbox_manual.md)

## Analysis Workshop 操作

* [Analysis Workshop](analysis-workshop/README.md)
   * [软件界面介绍](analysis-workshop/interface.md)
   * [Admin管理后台之Engine配置](analysis-workshop/admin-engine.md)
   * [简单使用示例](analysis-workshop/simple-example.md)
   * [透视表](analysis-workshop/pivot.md)
   * [可视化](analysis-workshop/dash.md)
   * [使用窗口进行数据分析](analysis-workshop/window.md)
   * [复杂组合条件过滤](analysis-workshop/complex-filter.md)
   * [MySQL数据库配置](analysis-workshop/ds-mysql.md)
   * [Json字段展开](analysis-workshop/json-fields.md)
   * [用MLSQL为Analysis Workshop开发插件](analysis-workshop/aw-plugin.md)

* [MLSQL语言控制台](console/README.md)
   * [界面简介](console/interface.md)
   * [简单使用示例](console/simple-example.md)

## MLSQL语法以及编程教程

* [MLSQL语法手册](lang/README.md)
   * [Set语法](lang/set.md)
   * [Load语法](lang/load.md)
   * [Select语法](lang/select.md)
   * [Train/Run/Predict语法](lang/et_statement.md)
   * [Register语法](lang/register.md)
   * [Save语法](lang/save.md)
   * [宏语法(命令行)](lang/macro.md)
   * [Include语法](lang/include.md)
   * [分支语句](http://blog.mlsql.tech/blog/mlsql-ifelse.html)
   * [MLSQL语法解析接口](lang/analyze.md)

* [MLSQL批处理编程](batch/README.md)
   * [MLSQL数仓/数据湖使用](datahouse/README.md)
       * [Hive加载和存储](datahouse/hive.md)
       * [Delta加载和存储以及流式支持](datahouse/delta.md)
       * [MySQL Binlog同步](datahouse/binlog.md)
   * [加载和存储多种数据源](datasource/README.md)
       * [JDBC](datasource/jdbc.md)
       * [ElasticSearch](datasource/es.md)
       * [Solr](datasource/solr.md)
       * [HBase](datasource/hbase.md)
       * [MongoDB](datasource/mongodb.md)
       * [Parquet/Json/Text/Xml/Csv](datasource/file.md)
       * [jsonStr/script/mlsqlAPI/mlsqlConf](datasource/mlsql_source.md)
   * [内置常见UDF](system_udf/README.md)
       * [http请求](system_udf/http.md)
       * [常见函数](system_udf/vec.md)

* [MLSQL流编程](stream/README.md)
   * [Kafka和MockStream](stream/datasource.md)
   * [MLSQL Kafka小工具集锦](stream/kakfa_tool.md)
   * [自动将Kafka中的JSON数据展开为表](stream/data_convert.md)
   * [如何高效的AdHoc查询Kafka](stream/query_kafka.md)
   * [如何设置流式计算回调](stream/callback.md)
   * [如何对流的结果以批的形式保存](stream/batch.md)
   * [window/watermark的使用](stream/window_wartermark.md)
   * [如何使用MLSQL流式更新MySQL数据](stream/stream_mysql_update.md)
   * [流结果输出到WebConsole](stream/web_console.md)

* [MLSQL机器学习编程](ml/README.md)
   * [特征工程](feature/README.md)
       * [文本向量化](feature/nlp.md)
           * [TFIDF](feature/tfidf.md)
           * [Word2Vec](feature/word2vec.md)
       * [特征平滑](feature/scale.md)
       * [归一化](feature/normalize.md)
       * [混淆矩阵](feature/confusion_matrix.md)
       * [QQ/电话/邮件抽取](feature/some_extract.md)
       * [离散化](feature/discretizer/README.md)
           * [Bucketizer](feature/discretizer/bucketizer.md)
           * [Quantile](feature/discretizer/quantile.md)
       * [Map转化为向量](feature/vecmap.md)
       * [数据集切分](feature/rate_sample.md)
   * [MLSQL Python支持](python/README.md)
       * [环境依赖](python/env.md)
       * [数据处理](python/etl.md)
       * [模型训练](python/train.md)
       * [PyJava API简介](python/pyjava.md)
       * [结合Python读取Excel](python/read_excel.md)
       * [结合Python保存Excel](python/write_excel.md)
       * [K8s下的Python资源限制](python/resource.md)
       * [dataMode 详解](python/datamode.md)
       * [Python并行度你所需要知道的](python/py_paralell.md)
   * [MLSQL内置算法](algs/README.md)
       * [KMeans](algs/kmeans.md)
       * [NaiveBayes](algs/naive_bayes.md)
       * [ALS](algs/als.md)
       * [RandomForest](algs/random_forest.md) 
       * [LogisticRegression](algs/logistic_regression.md)
       * [LinearRegression](algs/linear_regression.md)
       * [LDA](algs/lda.md)
       * [XGBoost](algs/xgboost.md)
   * [基于Java的深度学习框架集成](dl/README.md)
       * [加载图片数据](dl/load_image.md)
       * [Cifar10示例](dl/cifar10.md)
   * [部署算法API服务](api_deploy/README.md)
       * [设计和原理](api_deploy/design.md)
       * [部署流程](api_deploy/case.md)

* [MLSQL动态创建UDF/UDAF](udf/README.md)
   * [Python UDF](udf/python_udf.md)
   * [Scala UDF](udf/scala_udf.md)
   * [Scala UDAF](udf/scala_udaf.md)
   * [Java UDF](udf/java_udf.md)

## MLSQL 常见Native插件

* [计算复杂的父子关系](process/estimator_transformer/TreeBuildExt.md)
* [改变表的分区数](process/estimator_transformer/RepartitionExt.md)
* [如何发送邮件](process/estimator_transformer/SendMessage.md)
* [数据采集组件mlsql-watcher使用](process/estimator_transformer/mlsql-watcher.md)
* [语法解析SyntaxAnalyzeExt使用](process/estimator_transformer/SyntaxAnalyzeExt.md)
* [JSON展开JsonExpandExt使用](process/estimator_transformer/JsonExpandExt.md)

## 安全与隐私

* [安全与隐私](security/sum.md)
   * [MLSQL Engine 接口访问控制](security/README.md)
       * [接口访问Token设置](security/token_control.md)
       * [自定义接口访问策略](security/custom_control.md)
   * [授权用户对数据的访问控制](security/sum2.md)
       * [解析时表权限](security/compile_time.md)
       * [运行时表/列权限](security/runtime_time.md)

## 性能与资源

* [动态资源调整](resources/dynamic_resource.md)


## 插件/API/商店

* [MLSQL 脚本商店和插件](store/README.md)
   * [脚本插件save_excel](store/save_excel.md)
   * [MLSQL Engine插件](plugin/README.md)
      * [网络安装插件](plugin/online_install.md)
      * [离线安装插件](plugin/offline_install.md)
      * [使用MLSQL语言编写Spark程序](plugin/execute_mlsql_script.md)

* [API on（Console/Engine）介绍](api/sum.md)
    * [MLSQL Console API指南](developer/README.md)
       * [脚本获取接口](developer/script_api.md)
       * [脚本执行代理接口](developer/script_run_api.md)
    * [MLSQL Engine Rest接口详解](api/README.md)
       * [脚本执行接口](api/run-script.md)
       * [代码提示接口](api/code_suggest.md)
    * [MLSQL Engine Liveness探针](resources/liveness.md)
    * [MLSQL Engine Readness探针](resources/readiness.md)

## FAQ

* [常见问题](qa/README.md)
    * [文件上传失败怎么办](qa/upload_file.md)
    * [个人主目录是个啥](qa/home.md)
    * [会话隔离/并发执行/调试执行/定时任务](qa/session_isolated.md)
    * [CDH/HDP 怎么运行MLSQL Engine](qa/cdh_hdp.md)
    * [排查错误，三个系统的日志你都要看](qa/debug_log.md)
    * [听说mlsql-cluster暂时不更新了，mlsql-cluster是个啥？](qa/mlsql_cluster.md)
    * [MLSQL K8s部署，镜像环境如何制作](qa/mlsql-docker-image.md)
    * [写SQL如何避免拷贝黏贴](https://zhuanlan.zhihu.com/p/138405931)
    * [如何将SQL封装成命令调用](https://zhuanlan.zhihu.com/p/138475580)
    * [加载JDBC(如MySQL，Oracle)数据常见困惑](qa/load_jdbc.md)
* [最佳实践]()

## 开发者指南

* [MLSQL Engine开发环境设置](dev_guide/engine/README.md)
    * [Spark 2.4.3开发环境](dev_guide/engine/spark_2_4_3.md)
    * [Spark 3.0.0开发环境](dev_guide/engine/spark_3_0_0.md)    
* [ET插件开发](dev_guide/engine/plugin/ET_README.md)
    * [ET插件开发](dev_guide/engine/plugin/et.md)
    * [命令行开发](dev_guide/engine/plugin/et_command.md)    
* [自动化测试用例开发](dev_guide/engine/it/integration_test.md)     
* [其他插件开发](dev_guide/engine/plugin/OTHER_README.md)
    * [自定义数据源插件开发](dev_guide/engine/plugin/ds.md)
* [如何贡献代码](dev_guide/contribute.md)    

## 附录

* [常见宏命令](extra/commands.md)
