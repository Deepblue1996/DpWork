![Image text](https://raw.githubusercontent.com/Deepblue1996/DpWork/master/ic_logo.png)

<a href="http://developer.android.com/index.html"><img src="https://img.shields.io/badge/platform-android-green.svg"></a>
[![](https://jitpack.io/v/Deepblue1996/Bun.svg)](https://jitpack.io/#Deepblue1996/Bun)
<a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/badge/license-apache-green.svg"></a>

DpWork是一款便捷的应用程序开发框架。

### [不是开源的，只供使用]

[[中文文档]](https://github.com/Deepblue1996/DpWork/blob/master/README_CN.md)

## 如果使用

第一步:

创建并打开 Application Class,

必须继承 DpWorkApplication，重写

<pre><code>@Override
@DpBugly(id = "")
protected void initApplication() {

}
</code></pre>

第二步:

创建 public class WorkCore extends DpWorkCore，并重写

<pre><code>@Override
@DpInit(core = *.class)
protected void initCore() {
}
</code></pre>

## 基础配置

要在构建中加入Git项目:

步骤1.

在根Gradle中, repositories里添加:

	allprojects {
	    repositories {
		...
		maven { url 'https://jitpack.io' }
		maven { url 'https://dl.bintray.com/zchu/maven/' }
       	maven { url "https://raw.githubusercontent.com/Deepblue1996/DpWork/master" }
	    }
	}
步骤2. 添加依赖关系

	dependencies {
	        compile 'com.deep:DpWork:2.0.0'
	}
步骤3. 修改AndroidManifest，全面屏适配，基础修改，样式

    <meta-data
        android:name="android.max_aspect"
        android:value="2.1" />
步骤4. 使用混淆，可参考这里的 proguard-rules.pro

步骤5. Gradle

## LICENSE

<pre><code>Copyright 2018 Deepblue

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
</code></pre>
