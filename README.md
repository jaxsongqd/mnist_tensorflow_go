# mnist_tensorflow_go
golang 实现 部署 tensorflow model

#部署

1. 生成 model, 根据tensorflow 官方文档，使用[mnist的例子](https://tensorflow.google.cn/serving/serving_basic)
2. 启动 tensorflow_model_server
  可以使用bazel build 或者直接 apt-get install, 参考 [官方文档](https://tensorflow.google.cn/serving/serving_advanced)
3. golang 调用grpc 去调用tensorflow 的model

ps:话说，明明是个4 的图片， grpc调用给的结果，9这个数字的概率更大，。。。
