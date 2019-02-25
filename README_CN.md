![Image text](https://raw.githubusercontent.com/Deepblue1996/DpWork/master/ic_logo.png)

<a href="http://developer.android.com/index.html"><img src="https://img.shields.io/badge/platform-android-green.svg"></a>
[![](https://jitpack.io/v/Deepblue1996/Bun.svg)](https://jitpack.io/#Deepblue1996/Bun)
<a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/badge/license-apache-green.svg"></a>

DpWork是一款Android应用程序开发框架, 简单，便捷，集合

采用 - 单Activity+ 多Fragment框架设计

支持自适应布局，高自定义弹窗支持，网络层Dove，图片框架glide,
openGL音频媒体播放，实用工具类集合，内置国际化语言选择，支持高级防闪退机制等

欢迎加入QQ群: 257015764

### <a href="https://github.com/Deepblue1996/DpWorkDemo">查看使用示例源码(java-AndroidStudio2.3.3)</a>
### <a href="https://github.com/Deepblue1996/KotlinDpWork">查看使用示例源码(kotlin-AndroidStudio3.0+)</a>

[[English document]](https://github.com/Deepblue1996/DpWork/blob/master/README.md)

## 如果使用

第一步:

创建并打开 Application Class,

继承 DpWorkApplication，然后添加类注解

<pre><code>@DpBugly(id = "")
</code></pre>

第二步:

创建 public class WorkCore extends DpWorkCore, 然后添加类注解

<pre><code>@DpInit(core = *.class)
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

    Android Studio 2.3.3:
	dependencies {
	        compile 'com.deep:DpWork:2.2.3'
	}

	Android Studio 3.0+:
    implementation 'com.android.support:multidex:1.0.3'
    implementation('com.deep:DpWork:2.2.3') {
        exclude module: 'support-v4'
        exclude group: 'com.android.support'
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
