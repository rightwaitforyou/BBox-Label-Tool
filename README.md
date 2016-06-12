BBox-Label-Tool
===============

A simple tool for labeling object bounding boxes in images, implemented with Python Tkinter.

Data Organization
-----------------
LabelTool  
|  
|--main.py   *# source code for the tool*  
|  
|--Images/   *# direcotry containing the images to be labeled*  
|  
|--Labels/   *# direcotry for the labeling results*  
|  
|--Examples/  *# direcotry for the example bboxes*  

Dependency
----------
python 2.7 win 32bit
PIL-1.1.7.win32-py2.7


PIL The _imaging C module is not installed

今天在WIN 7 64位用PIL的时候，提示 The _imaging C module is not installed ，原来是需要安装64位的。

刚开始安装的是这个：http://www.pythonware.com/products/pil/  

但如果是64位，需要安装这：


Pillow-2.1.0.win-amd64-py2.7.‌exe 

http://www.lfd.uci.edu/~gohlke/pythonlibs/#pil
 

在python后输入
import ImageFont
如果不出错就OK了。。

在UBtunu下暂时还没遇到问题。 在公司的电脑也没遇到这问题。不过Google了发现很多人遇到这问题。记录一下

 

ubtunu 安装PIL ： 可用如下

sudo apt-get install python-imagingPIL The _imaging C module is not installed

今天在WIN 7 64位用PIL的时候，提示 The _imaging C module is not installed ，原来是需要安装64位的。

刚开始安装的是这个：http://www.pythonware.com/products/pil/  

但如果是64位，需要安装这：


Pillow-2.1.0.win-amd64-py2.7.‌exe 

http://www.lfd.uci.edu/~gohlke/pythonlibs/#pil
 

在python后输入
import ImageFont
如果不出错就OK了。。

在UBtunu下暂时还没遇到问题。 在公司的电脑也没遇到这问题。不过Google了发现很多人遇到这问题。记录一下

 

ubtunu 安装PIL ： 可用如下

sudo apt-get install python-imaging

Startup
-------
$ python main.py

Usage
-----
1. Input a number (e.g, 1, 2, 5...), and click 'Load'. The images along with a few example results will be loaded.
2. To create a new bounding box, left-click to select the first vertex. Moving the mouse to draw a rectangle, and left-click again to select the second vertex.
  - To cancel the bounding box while drawing, just press <Esc>.
  - To delete a existing bounding box, select it from the listbox, and click 'Delete'.
  - To delete all existing bounding boxes in the image, simply click 'ClearAll'.
3. After finishing one image, click 'Next' to advance. Likewise, click 'Prev' to reverse. Or, input the index and click 'Go' to navigate to an arbitrary image.
  - The labeling result will be saved if and only if the 'Next' button is clicked.
