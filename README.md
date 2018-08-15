
## 该项目主要用于文件的预览，使用springboot搭建
## 支持预览文件的类型
* 文本文件 如 txt | sql | java | js | html | xml | html | css 等
* 图像文件 如 jpeg | jpg | png | bmp 等
* 压缩文件 如 zip | rar | jar | gzip 等
* office文件 如 doc | docx | xlsx | xls | ppt | pptx 等
* pdf文件

## 使用方法
* 拉取项目到本地
* 下载并安装openoffice，在项目application.yml文件中配置openoffice的安装路径
* 造一个文件的下载地址，例如七牛云外链：http://p7ob9suqn.bkt.clouddn.com/layer-v3.1.1.zip （文件上传到七牛云仓库即可）
* 运行FileConventerApplication，启动项目，访问地址为：localhost:(端口号)/fileConventer?filePath=http://p7ob9suqn.bkt.clouddn.com/layer-v3.1.1.zip

## 转换规则
* 图片不进行转换,使用viewer.js展示
* 文本文件转换编码为utf-8
* office文件选择将word文档转为pdf文件，xls表格转为html文件，ppt文件转为图片
* 压缩文件先解压到本地，再利用Ztree插件（一个很强大的文件展示插件）做前端的展示

## 文件预览效果
> 压缩文件
![输入图片说明](https://github.com/Chenchicheng/file_viewer/blob/master/file-conventer/src/main/resources/static/images/compress.png "压缩文件预览.png")

> excel文件
![输入图片说明](https://github.com/Chenchicheng/file_viewer/blob/master/file-conventer/src/main/resources/static/images/excel.png "excel文件预览.png")

> word文件
![输入图片说明](https://github.com/Chenchicheng/file_viewer/blob/master/file-conventer/src/main/resources/static/images/paper.png "word文件预览.png")

> ppt文件
![输入图片说明](https://github.com/Chenchicheng/file_viewer/blob/master/file-conventer/src/main/resources/static/images/ppt.png "ppt文件预览.png")

> 图片
![输入图片说明](https://github.com/Chenchicheng/file_viewer/blob/master/file-conventer/src/main/resources/static/images/image.png "图片预览.png")

