### 3.2 编译本地HMI应用

&emsp;&emsp;本章节主要讲述MEasy本地HMI的编译过程。

&emsp;&emsp;我们提供MEasy本地HMI源码位于光盘文件的_/04-Linux\_Source/MEasy\_HMI/mxde.tar.gz_目录，将mxde.tar.gz拷贝到ubuntu目录工作目录，并解压出来。

&emsp;&emsp;下面讲述如何将mxde这个工程导入到QT Creator中，打开QT Creator，在菜单栏中依次点击`File`-&gt;`Open File or Project`然后弹出如图3-2-1 选择框，进入mxde工程目录，点击`mxde.pro`并点击`Open`按钮即可打开mxde这个工程。
{% raw %}
<div  align="center" >
<img src="/imagech/3-4-1.png",alt="cover", width=480 >
</div>
<div align="center" > 图3-2-1 工程选择框 </div>
<p></p>
{% endraw %}  

&emsp;&emsp;打开工程后进入配置页面，选择编译工具链，这里直接选择3.1章配置好的kits，点击`Configure Project`按钮然后进入工程目录。
{% raw %}
<div  align="center" >
<img src="/imagech/3-4-2-kits.png",alt="cover", width=480 >
</div>
<div align="center" > 图3-2-2 配置kits </div>
<p></p>
{% endraw %}  

&emsp;&emsp;进入mxde工程后即可看到整个工程的目录结构，如图3-2-3所示。然后可以对工程进行编译了，编译之前可以选择下编译输出的模式，这里我们选择Release模式，然后可以选择右下角小锤子图标进行编译整个工程，或者通过点击菜单栏`Build`-&gt;`Build Project "mxde"`,进行编译整个工程。
{% raw %}
<div  align="center" >
<img src="/imagech/3-4-3.png",alt="cover", width=480 >
</div>
<div align="center" > 图3-2-3 工程目录 </div>
<p></p>
{% endraw %}  

&emsp;&emsp;编译过程会可以从底部Table栏`4 Compile Output`中看到，如图3-2-4所示。
{% raw %}
<div  align="center" >
<img src="/imagech/3-4-4compile.png",alt="cover", width=480 >
</div>
<div align="center" > 图3-2-4 编译输出 </div>
<p></p>
{% endraw %}  

&emsp;&emsp;编译中出现的错误和警告信息可以从底部Table栏`1 Issues`中看到，如图3-2-5所示。如果编译出错可以从这里输出来进行分析问题。
{% raw %}
<div  align="center" >
<img src="/imagech/3-4-5 issues.png",alt="cover", width=480 >
</div>
<div align="center" > 图3-2-5 问题输出 </div>
<p></p>
{% endraw %}  

