# LaTeX-NewTemplate-For-NPU-Thesis
## 西北工业大学本科毕业设计新版本模板改动说明
 西北工业大学本科毕业设计新版本模板，根据https://github.com/polossk/LaTeX-Template-For-NPU-Thesis进行了调整
具体调整内容如下：
1. 修改了页眉页脚位置
2. 修复了行间距latex和word之间1.25倍行距的不同
3. 修改了字体为默认的宋体和黑体
4. 引用格式进行了进一步规范
5. 添加了一些引用公式、图片、列表、表格的示例

## latex环境配置
### 1. 安装texlive环境

阿里云镜像: https://mirrors.aliyun.com/CTAN/systems/texlive/Images/texlive.iso?spm=a2c6h.25603864.0.0.659d7002YwKsKh

加载iso文件，点击install-tl-windows.bat安装texlive环境即可。可以修改安装环境目录例如C:\texlive\2024

一路确定即可安装

### 2. 安装texstudio

官网: https://www.texstudio.org/

安装完成后，在选项-设置Texstudio-命令 中替换

Latex命令: 
```
"C:/texlive/2024/bin/windows/latex.exe" -src -interaction=nonstopmode %.tex
```

PdfLatex命令:
```
"D:/texlive/2024/bin/windows/pdflatex.exe" -synctex=1 -interaction=nonstopmode %.tex
```

XeLatex命令:
```
"D:/texlive/2024/bin/windows/xelatex.exe" -synctex=1 -interaction=nonstopmode %.tex
```

LuaLatex命令:
```
"D:/texlive/2024/bin/windows/lualatex.exe" -synctex=1 -interaction=nonstopmode %.tex
```

## 相关问题
### 关于编译问题
建议使用xelatex进行编译
### 关于文字比word版本细的问题
这个问题是由于latex文字渲染和word存在不同，质量不如word，建议使用Abode Acrobat重新打印一遍。

## 更新
- 2024.5.14 感谢@ouanneuzerl的PR，加入了添加了插图和表格列表的格式说明
- 2024.5.14 修改了nwpuname的字体路径问题，现在可以不用安装字体文件。并更新了readme文件

