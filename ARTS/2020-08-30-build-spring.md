# spring-framework-5.2.8 源码编译

## 1 准备

1. JDK1.8 +

2. Gradle

3. Jetbrains IDEA 社区或期间版

## 2 下载编译

1. [下载 spring-framework-5.2.8 源码压缩包](https://github.com/spring-projects/spring-framework/archive/v5.2.8.RELEASE.zip)

2. 预编译 spring-oxm `./gradlew :spring-oxm:compileTestJava`

3. Import 到 IDEA (File -> New -> Project from Existing Sources -> Navigate to directory -> Select build.gradle)

4. 排除 `spring-aspect` 模块

5. 刷新 gradle

## 3 常见问题

1. Gradle 下载太慢：

    手动先下载好对应版本的 gradle 压缩包，放入 dists 目录，如 `.gradle\wrapper\dists\gradle-5.6.4-bin`


2. Gradle 下载 jar 包失败

    手动下载好 jar 包放入 gradle 缓存目录(`.gradle\caches\modules-2\files-2.1`)
