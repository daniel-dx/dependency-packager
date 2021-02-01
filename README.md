# Sandpack Packager

> A packager used to aggregate all relevant files from a combination of npm dependencies

## Installing

This service is based on the services of Amazon. We use AWS Lambda, S3 and API Gateway to handle all requests. We provision these services using [serverless](https://serverless.com/).

Installation should be as simple as setting up serverless ([Getting Started](https://serverless.com/framework/docs/getting-started/)) and running `sls deploy --stage dev --s3prefix myBucketName`. `stage` can be either `prod` or `dev`, `s3prefix` is the prefix for your S3 bucket name.


## 如何开始

1. 安装依赖

```
$ yarn
```

2. 编译

```
$ yarn run build
```

3. 启动开发服务

```
$ yarn run dev
```

4. 访问调试链接: http://localhost:4545/[module name]@[version]

如：http://localhost:4545/lodash@latest

这样会请求 lodash 以及它的依赖的所有包代码
