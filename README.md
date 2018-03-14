# 天闻数媒WEB工程师入职指南
### 目录
1. 通用工具
2. 开发工具
3. 公司开发环境
4. 开发流程

 
# 通用工具
### RTX 

>公司目前的网络策略禁止在内网中使用QQ，微信等外部通讯工具。内部沟通使用RTX进行沟通。

下载RTX后，如下配置服务器设置，账号和密码可以从人事处获得。

![image](https://github.com/dingangang/web-/blob/master/RTX%E8%AE%BE%E7%BD%AE.jpg?raw=true)

### 公司邮箱

> 建议使用FoxMail。

下载安装以后，服务器配置如下图，邮箱的账号密码可以从人事处获取。

![image](https://github.com/dingangang/web-/blob/master/%E9%82%AE%E7%AE%B1%E8%AE%BE%E7%BD%AE.jpg?raw=true)




# 开发工具

### SVN

> 公司的文档管理使用SVN文件，目前公司的后台的代码进行了加密，前端组的文件暂时不需要加密和解密。

SVN的账号和密码在入职后咨询组长刘洁进行申请获取。

#### SVN工作原理

在一台服务器上建立一个源代码库，库里可以存放许多不同项目的源程序。由源代码库管理员统一管理这些源程序。每个用户在使用源代码库之前，首先要把源代码库里的项目文件下载到本地，然后开发人员可以在本地修改，左后用svn命令进行提交，由源代码库统一管理修改。

下载安装SVN以后，在空白文件夹中右键菜单中可以看到(仅列举了常用项目)：

    |- SVN Checkout                       该命令用于在当前文件夹下载服务器上存放的文档。
    |- TortoiseSVN
        |- Repo Browser                   该命令用于打开SVN自带的文档浏览器。

在已经Checkout的文件夹中，右键菜单变为：

    |- SVN Update                        将文件夹中与服务器中最新版本进行合并升级。
    |- SVN Commit                        提交修改的文件到服务器。
    |- TortoiseSVN
        |- Show log                      显示提交日志。
        |- Repo Browser                  自带浏览器。
        |- Resolve                       处理一些SVN不能判定的代码冲突，使用较少，通常和共同开发组员商议解决。
        |- Update to Revision            回滚到之前的版本，使用较少。
        |- Relocate                      切换工作目录，使用较少。现已经全部统一更换了路径。
        |- Add                           添加新增的文件，也可以直接执行Commit时进行相关操作。

#### 使用示例

> *http://192.168.111.244:8888/svn/aischool/doc/02.组织文档/06.UI组/05.KPI与绩效管理/2017/07.年度总结*
   
#### 下载文件   
    
复制上方链接，在本地空白文件夹中右键菜单中选择 SVN Checkout 命令。确定后即可将服务器上的内容下载到本地。对“员工总结-UI-丁昂昂.docx”进行了修改并保存。新增了文件“新增文件.docx”。

![image](https://github.com/dingangang/web-/blob/master/SVN%E7%A4%BA%E4%BE%8B.jpg?raw=true)

#### 文件状态

1. 与服务器上保持一致的文件状态为绿色的√标记。
2. 本地修改过的文件状态为红色！标记
3. 新增的文件状态为蓝色？标记

#### 上传文件

本地修改完成后，在文件夹右键菜单中选择 SVN Commit 

![image](https://github.com/dingangang/web-/blob/master/SVN%E7%A4%BA%E4%BE%8B1.jpg?raw=true)

修改过的文件和新增的文件出现在提交列表中，修改的文件已经自动勾选，新增的文件没有被勾选。

如果上传前对列表中“新增文件.docx”执行了SVN-->add操作，则同样会默认勾选。

直接选在SVN Commit时，可以选择提交列表上的ALL，全部进行选择，包含修改的、新增的和删除的文件。提交删除信息后，对应的文件在SVN库中也会被删除。

在Message中一般需要提交信息，模板如下：

    【版本】详细的项目版本名
    
    【单号】JIRA中可以对应的单号，非改单的情况可以用XXX-000来代替
    
    【描述】描述解决的问题
    


### IDE

> 使用自己习惯的IDE

#### WebStrom

是jetbrains公司旗下一款JavaScript 开发工具。各项功能都比较全，简要设置也可以支持Vue.js的开发。

#### Sublime Text

一款具有代码高亮、语法提示、自动完成且反应快速的编辑器软件。需要自己按需配置一些习惯的插件。

#### Visual Studio

是美国微软公司的开发工具包系列产品。VS是一个基本完整的开发工具集，它包括了整个软件生命周期中所需要的大部分工具。

### PxCook

> 利用PxCook可以很方便的查看图形元素的对应CSS信息，减少交流成本。

PxCook是一款辅助用的图形信息查看软件。运用PxCook可以很快的获取高保真文件中的元素的属性已经许多需要测量的间距。它支持读取各类图片文件和PhotoShop生成的SPD源文件。当读取PSD源文件的时候，PxCook提供的开发者模式甚至可以提供部分可以使用的CSS信息。开发过程中也从UI设计人员处获取PSD源文件的SVN地址。


# 公司开发环境

### 公司需求文档目录

> 公司的所有需求文档都上传在这个地址，直接使用浏览器打开即可。相关账号同SVN一致。

*http://192.168.102.222:9888/pages/viewpage.action?pageId=1179780*


### JIRA BUG处理系统

> BUG管理系统，在转测的时候进在此处进行BUG单处理协作。相关账号同SVN一致。

*http://192.168.102.222:8888/secure/Dashboard.jspa*

### 前端组开发目录

> 前端本地的开发目录，主要存放未编译的项目文件

*http://192.168.111.244:8888/svn/aischool/doc/02.组织文档/06.UI组/02.HTML文件/02.前端文件库/前端自动化目录*

在自己本地合适的磁盘，建立对应的文件夹后，可以将上方目录通过SVN Checout 到本地。

![image](https://github.com/dingangang/web-/blob/master/%E5%89%8D%E7%AB%AF%E5%BC%80%E5%8F%91%E7%9B%AE%E5%BD%95.jpg?raw=true)


### 项目交付目录

> 完成后项目交付目录，开发人员从此目录获取前端文件

*http://192.168.111.244:8888/svn/aischool/doc/01.项目文档/XXX*

直接下载01.项目文档可能会因文件过多出问题。

建议在本地磁盘按照对应的项目层级建立文件夹，方便查看管理。例如：

    |- 项目文档                          建立在本地的文件夹
        |- 走班制选课                    对应的项目名称
            |- V001R001C02              对应的版本
                |- 02.受控区 
                    |- 02.UI原型         前端交付文件夹 
                        |- 01.高保真     存放UI设计人员提供的图片、图标和规范
                        |- 02.HTML       web工程师提交的文件

![image](https://github.com/dingangang/web-/blob/master/%E9%A1%B9%E7%9B%AE%E6%96%87%E6%A1%A3.jpg?raw=true)

通常在SVN Repo Browser 中选取02.HTML，复制URL后在本地建立好的同结构文件夹中进行SVN Checkout。01.高保真是UI设计人员提供的高保真图片和切图。一般也会通过SVN Checkout 到本地。

# 开发流程

### 阅读需求文档

> 仔细阅读需求文档，是减少后续开发分歧的好办法。

*http://192.168.102.222:9888/pages/viewpage.action?pageId=1179780*

点击链接进去需求文档空间，根据SE提供的地址打开对应的需求文档。

需求文档的内容要仔细查看。对应的图片和一些逻辑也要仔细分析，特别是针对样式的部分要注意，一些前端可以完成的交互性的需求也需要在交付的文件中完成。

文档中高亮的地方是有人针对该处提出的疑问。可以进行查看，如果有自己不清楚的地方也可以自己左键选取文字后会弹出可以操作的按钮，点开后进行审评，并提出自己的意见。

### 需求审评

> 提出恰当的修改意见

需求文档下达以后会有审评会议，SE会负责讲解，开发人员可以针对需求提出疑问。Web工程师需要针对页面的样式和会需要编写的JS逻辑进行提问，说明意见及修改方案。

### 低保真文件

> SE 通过axure生成的项目描述文件。Chrome需要安装 Axure RP Extension for Chrome

低保真文件中描述了对应的一些功能需求，通常大的项目最后的实现效果和低保真会有一些不同，但是大致的功能是一致的。下图是一个低保真的示例，这个低保真是现有的项目上一些需要改变的需求。新项目的话低保真样式更简单一些。

![image](https://github.com/dingangang/web-/blob/master/%E4%BD%8E%E4%BF%9D%E7%9C%9F%E7%A4%BA%E4%BE%8B.jpg?raw=true)


### 高保真文件

> UI设计人员制造的最后想要呈现在用户面前的样本。

高保真文件通常格式为jpg或jpeg。是希望最后用户能看到的界面样本。

**web工程师最主要的任务就是将高保真文件所描述的界面转化为HTML、CSS和JavaScript共同构成的前端页面。**

![image](https://github.com/dingangang/web-/blob/master/%E9%AB%98%E4%BF%9D%E7%9C%9F%E7%A4%BA%E4%BE%8B.jpg?raw=true)

下方的图是该系统颜色设计规范。系统中的对应元素的配色都要按照规范来进行，可以的话也可以引入Sass,后续有颜色调整的情况也会方便一些。

![image](https://github.com/dingangang/web-/blob/master/%E9%AB%98%E4%BF%9D%E7%9C%9F%E7%A4%BA%E4%BE%8B2.jpg?raw=true)


### 本地工程简介

### 项目基础版本(非gulp)

> http://192.168.111.244:8888/svn/aischool/doc/02.组织文档/06.UI组/02.HTML文件/02.前端文件库/前端自动化目录/项目基础版本(非gulp)

这个文件夹中的部分项目是旧的项目，没有引入前端的一些新技术，就是最单纯的HTML、CSS和JavaScript。

项目结构为：
 
    |– 项目名称                  项目文件夹，存放HTML页面
        |-  其他需求页面         用于放一些拓展需求的页面
        |- css
            |- bootstrap        bootstrap工程或其他的一些第三方工程
            |- main             存放css文件
                |- images       存放图片
        |- js                   存放JS文件

示例项目对照：

![image](https://github.com/dingangang/web-/blob/master/%E9%A1%B9%E7%9B%AE%E7%BB%93%E6%9E%84%E7%A4%BA%E4%BE%8B.jpg?raw=true)

这些项目中编辑完后就直接覆盖提交到对应的交付目录了。有些文件是不用上传到SVN上去的，如上图中的.idea文件是WebStrom生成的配置文件，可以选定后右键TortiseSVN->Add to ignore list。这样以后的SVN Commit中都不会包含此文件夹。


### 教育云

> http://192.168.111.244:8888/svn/aischool/doc/02.组织文档/06.UI组/02.HTML文件/02.前端文件库/前端自动化目录/教育云

这是基于webGulpCom工程的项目，单独为ECP教育云项目设立的。此项目中引入了gulp。

#### node.js 和 cnpm

请先安装好node.js 并且安装好cnpm。 


#### 使用说明

gulp的引入目的在于提高前端代码的编写效率（注：本环境基于[nodejs](https://nodejs.org/en/)，所以请先安装好nodejs再运行本工程）。

    第一步： 如果没有安装过插件执行运行webGulpCom下的install.cmd进行安装，如果安装过，忽略第一步。
    第二步： 运行preject/demo中的run.cmd即可跑工程。

#### 重点关注的文件
    gulpfile.js                 gulp运行入口文件
    config.js                   环境的所有配置信息都在这
    install.cmd                 安装环境所有依赖插件
    run.cmd                     启动gulp工程，开启服务器
    publish.cmd                 发布工程到publish目录文件
    clean.cmd                   清除生成的目标文件

#### 环境目录结构
    |– gulp                          gulp相关的所有任务、配置文件信息
         |- tasks                    gulp的所有任务文件目录
              |- cssTask.js          css生成、修改、删除的相关任务
              |- htmlTask.js         html生成、修改、删除的相关任务
              |- imagesTask.js       图片生成、修改、删除的相关任务
              |- scriptsTask.js      JavaScript生成、修改、删除的相关任务
              |- sprinteTask.js      雪碧图相关任务（包括web、手机端）
              |- pugTask.js          将所有pug文件编译成html文件
              |- scssTask.js         编译scss文件为css文件(所有文件合并到main.scss，然后编译成main.css)
              |- othersTask.js       为除以上文件目录外的所有目录提供文件拷贝功能
              |- util.js             消息提示等工具任务
         |- config.js                配置文件（工程所有配置信息都在这）
         |- css.handlebars           web端雪碧图生成格式文件
         |- phoneCss.handlebars      手机端端雪碧图生成格式文件
         |- phoneFontCss.handlebars  纯手机端端雪碧图生成格式文件
         |- iChoice.handlebars       ichoice任务雪碧图生成格式文件
    |- node-modules                  node自动生成目录（所有安装本地插件都在这）
    |- project                       工程放置位置
    |- .csscomb.json                 css格式化格式(csscomb插件配置文件，可在官网直接生成，插件会自动调用，不需管)
    |- gulpfile.js                   gulp运行入口文件
    |- install.cmd                   插件安装运行文件
    |- package.json                  node工程依赖插件关系包
    |- postcss.config.js             postcss配置文件
    |- README.md                     说明文档
    |- README_plugins.MD             插件说明文档

#### 单个工程目录结构(demo工程为例)
    demo
    |- src                           源文件目录
        |-  version
            |-*.html                 所有html文件
        |- module                    html模块目录
        |- js                        工程相关js文件目录
        |- icons                     web端雪碧图源文件存放目录
        |- iconsphone                手机端雪碧图源文件存放目录(纯手机端也放在此目录下)
        |- css                       样式文件目录（包括css、scss）
            |- main
                |- images            教育云的图片都放在此处，针对教育云更改了配置。
                |- main.css          这一份main.css是旧时的main.css。编译过程中将main.scss编译后拼接了此份main.css作为dist中的输出main.css
        |- 其他                      支持其他目录创建（比如字体图标目录font）
    |- clean.cmd                     清除生成的目标文件
    |- publish.cmd                   发布工程到publish目录文件
    |- run.cmd                       启动gulp工程，开启服务器
    
#### main.scss

项目中main.css是主要的编译对象，是生成dist中main.css的主入口。在这个项目中，因为定制化的内容比较多，在C05版本时，将其他的内容进行了模块化，固定了一些原有的内容。后续进行新的需求开发，要在css文件夹中建立新的模块文件夹，并且引入到main.scss中。这样便于样式的管理，不会造成最后交付的main.css过于臃肿。

#### 雪碧图

**gulp.spritesmith** 是生成雪碧图的gulp插件。启动工程时，放在icons文件夹中的图片会合并成为一张整的图片，对应生成的 **_icons.scss** 也会自动根据图片的位置修改，不要去手动修改。图标在HTML文件中的使用方式如下：

    <i class="icon icon-XXX"><i/>
    
不同工程中或许略有差异，已当前的工程中的雪碧图命名为准。项目基础版本(非gulp)中没有用到雪碧图，一些图标的管理比较零散，修改时需要注意。

#### webGlup

> webGlup中使用的是旧版的gulp


##### 重点关注的文件
    config.js                   工程的所有配置信息都在这
    run.cmd                     启动gulp工程，开启服务器
    clean.cmd                   清除生成的目标文件

##### 目录结构
    |– gulp                          gulp相关的所有任务、配置文件信息
         |- tasks                    gulp的所有任务文件目录
              |- cssTask.js          css生成、修改、删除的相关任务
              |- htmlTask.js         html生成、修改、删除的相关任务
              |- imagesTask.js       图片生成、修改、删除的相关任务
              |- scriptsTask.js      JavaScript生成、修改、删除的相关任务
              |- sprinteTask.js      雪碧图相关任务
              |- util.js             消息提示等工具任务
         |- config.js                配置文件（工程所有配置信息都在这）
    |- node-modules                  node自动生成目录（所有安装本地插件都在这）
    |- project                       工程放置位置
    |- demo                          示例工程
    |- .csscomb.json                 css格式化格式(csscomb插件配置文件，可在官网直接生成，插件会自动调用，不需管)
    |- package.json                  node工程依赖插件关系包
    |- README.md                     说明文档
    |- README_plugins.MD             插件说明文档

#### 单个工程目录结构(demo工程为例)

    demo
    |- src                           源文件目录
    |- css                           css文件放置目录
        |- main                      自己新增的样式目录
            |- images                图片放置目录
            |- scss                  scss文件放置目录
            |- sprite                雪碧图放置目录
            |- main.css              样式主文件
    |- js                            js文件放置目录
    |- index.html                    html文件入口(可自行修改配置文件来定义)
    |- clean.cmd                     清除生成目录
    |- gulpfile.js                   gulp默认入口文件(开启gulp执行的第一个文件)
    |- run.cmd                       开启gulp工程，启动服务器
    
旧版gulp同样用到了 **gulp-content-includer**  、雪碧图和Sass。


### Vue.js项目

> http://192.168.111.244:8888/svn/aischool/doc/02.组织文档/06.UI组/02.HTML文件/02.前端文件库/前端自动化目录/VUE项目/数据同步监控平台

#### 目录结构

    |- build                         配置文件，不要改动
    |- config                        配置文件，不要改动
    |- cssTemplate                   雪碧图模板，不要改动
    |- src                           源文件目录
        |- assets                    资源文件
        |- components                组件存放的位置
        |- config
            |- register.js           全局组件注册
            |- router.js             vue-router配置
            |- store.js              vux相关配置
        |- pages                     用于存放页面
        |- static
            |- css                   CSS存放文件
            |- icons                 雪碧图图标
            |- images                图片
            |- plugs                 额外的插件
        |- App.vue                   程序入口组件    
        |- main.js                   程序主入口
    |- static                        实际的样式文件目录，执行x-ui.cmd交给gulp托管。
    |- dev.cmd                       打开webpack开发环境
    |- gulpfile.js                   gulp配置文件
    |- index.html                    入口html
    |- package.json                  项目描述文件
    |- start.bat                     同时打开webpack开发环境，和gulp托管。
    |- x-ui.cmd                      启动gulp托管CSS的编译工作

目前的VUE项目中，同时也使用了gulp来进行管理。webpack仅负责打包项目。项目主目录下的static文件夹相当于是gulp的dist目录。src->static中的内容会被编译到主目录下的static文件夹，项目中引用的样式文件也是直接从主目录下static中引入。


### JIRA BUG管理系统使用

> JIRA是在系统转测期间用于交流跟踪的系统

示例： *http://192.168.102.222:8888/browse/EBAG-78647*

EBAG-78647是该单对应的 **单号** 。

**问题详情** 中有版本信息和环境信息。

**描述** 中有找到对应该问题出现的操作。

**附件** 中会有对应问题的截图。

web工程师需要处理页面缺陷，按照 **描述** 中的操作找到对应的页面，分析页面缺陷原因，找出解决方法。常见的一些问题有：

    1. CSS缺陷：字符截断错误、图标未对齐错误、间距不符错误、字体及颜色错误等。这一类的错误不需要改动HTML元素，只需要在CSS文件中进行修改。
    2. JS缺陷： 这一类的错误部分在引入的JS文件中修改，部分在页面中修改。修改完成后要进行截图说明，告知开发修改的点。
    3. HTML结构问题：高保真HTML结构缺陷、开发使用HTML错误。这一类错误也需要截图说明需要修改的点。
    4. 兼容性问题: IE8或者不同的浏览器之间的错误。删除浏览器不支持的属性，需要主流的浏览器中保持一致的显示。这一类问题也要截图说明。
    5. 不明确的错误：这一类问题需要商讨解决，要寻找可替代的方案。
    
解决问题后，通常将截图上传到 **附件** ，涉及到文件修改替换的要及时上传到项目文档，并且告知开发人员对应的SVN地址的更新。

### 协作开发

> SVN库中，只会保留最新的一个版本

协作开发的时候要遵循：
    
    1. 避免开发人员共同开发同一文件
    2. 开发前需要时常更新本地代码库
    
**本地的开发环境保持一致的版本，交付的内容直接复制本地编译后的文件覆盖交付项目文件。**
    
假设有如下场景：

开发者：chenjinbin 和 dingangang。他们共同修改main.css,原始代码如下：

    body{
        background-color: #fff;
        height: 100%;
    }
    
chenjinbin修改了背景颜色,并且Commit了main.css

    body{
        background-color: #000;
        height: 100%;
    }
    
dingangang修改了高度

    body{
        background-color: #fff;
        height: 90%;
    }
    
dingangang进行Commit操作的时候会看到错误提示：

**提示开发者该文件已经过期，需要先更新文件**

![image](https://github.com/dingangang/web-/blob/master/%E6%96%87%E4%BB%B6%E8%BF%87%E6%9C%9F.jpg?raw=true)

执行Update，SVN会自动把其他用户修改的操作更新到该文件中（**前提是不同用户修改的位置不同**），并且**保存当前用户修改的部分**。

dingangang执行Update以后，会发现main.css已经变成：

    body{
        background-color: #000;
        height: 90%;
    }
    
再次进行提交，提示成功。

所以，如果必须两人或多人开发同一个文件，建议先如下布局，各自只修改自己区域的代码

    /************ cehenjinbin ************/
    ...
    chenjinbin的代码
    ...
    /************ cehenjinbin end ************/
    /************ dingangang ************/
    ...
    dingangang的代码
    ...
    /************ cehenjinbin end ************/
    
如果不慎造成了冲突*conflicted state*（**应当避免这种情况**），直接与其他人员进行协商沟通，更新版本库中的内容。不要自己直接处理conflicted从而造成更多的问题。
    
如果可以拆分成多个文件，则各自负责开发自己的部分。每次进行提交前先执行一次Update。