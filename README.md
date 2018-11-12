![Image text](https://raw.githubusercontent.com/Deepblue1996/DpWork/master/ic_logo.png)

<a href="http://developer.android.com/index.html"><img src="https://img.shields.io/badge/platform-android-green.svg"></a>
[![](https://jitpack.io/v/Deepblue1996/Bun.svg)](https://jitpack.io/#Deepblue1996/Bun)
<a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/badge/license-apache-green.svg"></a>

DpWork is a convenient application development framework.

### [not open source, only available for use]

[[中文文档]](https://github.com/Deepblue1996/DpWork/blob/master/README_CN.md)

## How do I use Bun

One:

Create or open your Application Class, 

You must extend DpWorkApplication

<pre><code>@Override
protected String buglyId() {
    return "";
}
</code></pre>

Two:

Create public class WorkCore extends DpWorkCore

<pre><code>@Override
protected IBaseScreen mainScreen() {
    return DemoFirstScreen.newInstance(); // Screen
}
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
       		maven { url "https://raw.githubusercontent.com/Deepblue1996/DpWork/master" }
	}
	}
Step 2. Add the dependency

	dependencies {
	        compile 'com.deep:DpWork:1.0.0'
	}
Step 3. Gradle

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
