<h3>一、前言</h3>

&nbsp;&nbsp;在学习vue期间，感受到vue开发组件化、模块化的spa项目，具有很高灵活性、可读性。当然这种灵活性一方面有利于我们自由发挥扩展，一方面同时要考虑如何利用好vue的灵活性，推动项目的快速开发、迭代。

&nbsp;&nbsp;这次主要是为了学习在vue中如何进行css模块化，实现基本组件的最大复用，基本组件和业务组件分离，达到高度的可复用性，这就需要我们在设计的时候兼顾灵活性、扩展性。如果想学习vue全家桶的使用可以查看我的`vue-music-project`

[vue-music-project github地址传送门](https://github.com/jiaen188/vue-music-project)


<hr/><h3>二、技术栈</h3>

    vue + vue-router + sass

<h3>三、vue-cli 环境搭建</h3>

``` bash
git clone git@github.com:jiaen188/vue-jingdong-project.git

cd vue-jingdong-project

npm install

npm run dev
```

<hr><h3>四、目录结构</h3>

```
|——app	
	|——css                                 //样式
|	
	|——js——                                //组件 
|	    |——core                            //核心组件
	|       |——btn.vue                     //按钮组件
|       |
    |       |——panel.vue                   //板块组件
|       |
    |       |——slider.vue                  //轮播图组件
|
    |
|		|——home                            //首页面板
	|	
|		|——ious                            //白条面板
	|	
|		|——money                           //理财面板
	|		
|		|——public                          //公共组件
	|			
|		|——raise                           //众筹面板
	|		
|		|——router                          //路由
    |       |——index.js
|       |
    |
|		|——special                          //活动页面板
	|
|		|——App.vue                          //主文件
	|
|		|——main.js                          //主文件路由
	|	
|		|——viewport.js                      //移动端自适应文件
	|	
|	
	|——view——                               //首页	
        |——index.html                                    
|

```