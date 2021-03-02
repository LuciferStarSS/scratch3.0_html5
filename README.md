# scratch3.0_html5
An HTML5 version of Scratch3.0 Editor, which based on the official Node.js edition ( https://github.com/LLK/scratch-www ).
Just download all the files, and browse the file ./editor/Scratch3.0.html in any webpage browsers which support HTML5, and in any operating systems.
NO Internet Explorer.

IT WORKS WELL ON MY CHROMEBOOK!

Scratch3.0(HTML5)学习平台

本程序基于MIT开源的scratch-www项目，经修改而来。其中，所有图片和声音资源，版权都属于Scratch官方，而程序，则遵循scratch-www原有的开源协议。


原本的scratch-www项目，基于Node.js，需要部署在支持Node.js的服务器上，运行服务器端程序后，用户通过支持HTML5的浏览器才可访问。
其中，角色和背景的图片资源，以及文字朗读、翻译两个扩展模块中的功能，需要访问Scratch官网服务器，才可实现功能。
而由于Scratch官方社区被信息污染导致无法正常访问，所以上述资源已不能正常访问。

由于Node.js应用，虽然生成于远程服务器之上，但客户端在运行时，所有程序和数据应该是都在浏览器里的，所以，我尝试着剥离该套程序对Node.js的依赖，并最终获得了成功。
在此，要感谢 https://github.com/open-scratch/scratch-asset-utils 提供的从Scratch官方爬回的图片资源（有几个角色的图片错误了，只好手动修正）。

制作这个版本，本是出于无奈。
最初的1.4，安装繁琐，且会崩溃，导致数据丢失。
正好看到MIT的开源项目scratch-flash，于是我做了一个PHP+FLASH的Scratch2.0网站平台，在那个平台里，每一个修改，都可以触发服务器端的自动备份操作。
然而，FLASH还是亡了。
最终，HTML5版，就这样诞生了。
希望，HTML5版，能活久一点。

注：
“./editor/js/projects.bundle.js”官方是15MB多点，我这个，有95MB，因为把所有图片和声音，都内置了。
这样处理，坏处就是文件太大，而好处，就是不需要架设服务器，直接用浏览器打开“./editor/Scratch3.0.html”，就可以用了。
安卓、iOS，手机、平板，安逸。
