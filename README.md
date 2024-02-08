# <p align="center">Latex template for thai language </p>

### สิ่งที่ต้องรู้เบื้องต้น

#### Compiler

latex เปรียบเสมือน Markup language ที่ต้องการ compile เพื่อเป็น pdf ดังนั้นต้องใช้เครื่องมืออยู่ 3 อย่าง

1. **Compiler** ที่จะทำการแปลงไฟล์ latex ให้ออกมาในรูปของ pdf
    - Linux - TexLive
    - Windows - MikTeX
    - Mac OS - MacTeX

    compiler มีอยู่หลายตัว สามารถใช้ตัวอื่นก็ได้

2.  นอกจากจะมี **Compiler** มาแล้ว ก็จะมีตัว packager manage มาให้ด้วย เพื่อใช้สำหรับติดตั้ง package

3. **Editor** ก็คือโปรแกรมที่ใช้ในการเขียน latex ซึ่งมีอยู่หลายตัวเช่น `TexStudio` หรือจะใช้ `Vscode` ก็ได้ เพราะเป็นเพียงการแก้ไข text file เท่านั้น

- หากจะใช้เขียนภาษาไทยต้องใช้ package `fontspec` และเซ็ต mainfont เป็นฟ้อนต์ไทย
- หากใช้เขียนภาษาไทยด้วย `vscode` ต้องมีการตั้งค่าเพิ่มเติม [อ่านได้ที่นี่](https://medium.com/@kritsiwat/%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B8%84%E0%B8%B3%E0%B8%AA%E0%B8%B1%E0%B9%88%E0%B8%87-xelatex-%E0%B8%9A%E0%B8%99-visual-studio-code-%E0%B9%82%E0%B8%94%E0%B8%A2%E0%B9%83%E0%B8%8A%E0%B9%89-plugin-latex-workshop-d6462cb5af46)

### ตัวอย่าง texlive บน Linux

ติดตั้ง texlive

```
$ sudo pacman -S texlive-basic texlive-meta
```
compile ไฟล์ latex เป็น pdf

```
$ xelatex filename.tex
```

ติดตั้ง package

```
$ sudo tlmgr install fontspec  
```


# Inside it
 
- THSarabunNew