![Image text](https://raw.githubusercontent.com/Deepblue1996/DpWork/master/ic_logo.png)

<a href="http://developer.android.com/index.html"><img src="https://img.shields.io/badge/platform-android-green.svg"></a>
[![](https://jitpack.io/v/Deepblue1996/Bun.svg)](https://jitpack.io/#Deepblue1996/Bun)
<a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/badge/license-apache-green.svg"></a>

DpWork is an Android application development framework that is simple, convenient and comprehensive

Adopt - single Activity+ multi Fragment frame design

Support for adaptive layouts, high custom popup support, network layer Dove, image frame glide,
OpenGL audio media playback, utility class set, built-in internationalization language selection, support advanced anti - flashback mechanism

Welcome to QQ group: 257015764

### See using sample source code - <a href="https://github.com/Deepblue1996/DpWorkDemo">java-AndroidStudio2.3.3</a>/<a href="https://github.com/Deepblue1996/QiaoQiao">kotlin-AndroidStudio3.0+/瞧瞧</a>

[[中文文档]](https://github.com/Deepblue1996/DpWork/blob/master/README_CN.md)

## How do I use DpWork

One:

Create or open your Application Class, 

You must extend DpWorkApplication, then add the class annotation

<pre><code>@DpBugly("Bugly id")
</code></pre>

Two:

Create public class WorkCore extends DpWorkCore, then add the class annotation

<pre><code>@DpInit(*.class) // FirstScreen Name
</code></pre>

## Basic deployment

To get a Git project into your build:

Step 1. Add the JitPack repository to your build file

gradle
maven
sbt
leiningen
Add it in your root build.gradle at the end of repositories:

	allprojects {
	    repositories {
		...
		maven { url 'https://jitpack.io' }
		maven { url 'https://dl.bintray.com/zchu/maven/' }
       	maven { url "https://raw.githubusercontent.com/Deepblue1996/DpWork/master" }
	    }
	}
Step 2. Add the dependency

    Android Studio 2.3.3:

	dependencies {
	    compile 'com.deep:DpWork:2.4.5'
	}

	Android Studio 3.0 +:

    implementation 'com.android.support:multidex:1.0.3'
    implementation('com.deep:DpWork:2.4.5') {
        exclude module: 'support-v4'
        exclude group: 'com.android.support'
    }

Step 3. For confusion, refer to proguard-rules.pro here

Step 4. Gradle

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


