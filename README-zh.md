## SubmitButto

[![Travis](https://img.shields.io/badge/download-1.0.1-brightgreen.svg)](https://bintray.com/unstoppable/maven/submitbutton/1.0.1)


README: [English](https://github.com/Someonewow/SubmitButton/blob/master/README.md) | [中文](https://github.com/Someonewow/SubmitButton/blob/master/README-zh.md)



>带有Loading的Android自定义View.

## 示例

![submit succeed](http://oop9jkflc.bkt.clouddn.com/submitbutton_01.gif)

![submit failed](http://oop9jkflc.bkt.clouddn.com/submitbutton_02.gif)

## 如何使用

##### 1.在要使用的Module的build.gradle文件中添加依赖;

	dependencies {
		'''
    	compile 'com.unstoppable:submitbutton:1.0.1'
	}

##### 2.布局文件中添加SubmitButton;

	<com.unstoppable.submitbuttonview.SubmitButton
        android:id="@+id/submitbutton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content" />

##### 3.自定义属性

| 属性名        | 类型      | 描述               |默认值    |
|:--------------|:-----    |:------------------|:----    |
|buttonColor    |color     |按钮主题色           | #19CC95 |
|buttonText     |String    |按钮文本            |null     |
|buttonTextSize |dimension |按钮文本大小         |15sp    |
|succeedColor   |color     |submit成功按钮主题色 | #19CC95 |
|failedColor    |color     |submit失败按钮主题色 | #FC8E34 |

##### 4.接口方法
	
	 /**
     * 传入submit结果以呈现不同结果反馈效果
     *
     * @param boolean isSucceed 
     */
	mSubmitView.doResult(isSucceed);

	 /**
     * 重置SubmitButton 
     */
	mSubmitView.reset();

## License

	Copyright 2017 Unstoppable

	Licensed under the Apache License, Version 2.0 (the "License");
	you may not use this file except in compliance with the License.
	You may obtain a copy of the License at

	   http://www.apache.org/licenses/LICENSE-2.0

	Unless required by applicable law or agreed to in writing, software
	distributed under the License is distributed on an "AS IS" BASIS,
	WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
	See the License for the specific language governing permissions and
	limitations under the License.