#### 0.1
    ##### 1.项目开始
#### 0.2
    1.可以针对不同形状的零件（接管，圆板，环板）生成DXF文件
#### 0.3
    1.支持读取Excel文件，自动生产相对应的dxf文件
    2.新增加一种零件（方板类）的dxf自动生成
#### 0.4
    1.新增加对于波纹管数据直接转换dxf文件
#### 0.5
    1.特殊尺寸的波纹管可以直接输出重量
    2.不同厚度的材料将自动生成至各自的文件夹
    3.默认查找该文件夹下以 "排料清单.xlsx" 结尾的excel进行排料
#### 0.6
    1.excel模板修改，新增加项目材料，调整厚度的位置
    2.不同厚度和材料的板材可生成各自的文件夹
    3.为该项目设计了简陋的图形界面
#### 0.7
    1.支持一键生成下料清单
    2.修复一些BUG
#### 0.8
    1.修复一重要BUG，

#### 1.0
    1.将程序分为6个模块，重构了部分代码，新增加以号代图识别模块
    2.可以识别设计直接导出的excel清单，简单修改后即可开始排料
    3.以号代图可以识别种
    4.一次性可以输入个excel表格，输出文件在选定excel表格的文件中
    5.修复多个重要Bug

#### 1.1 todo
    修改图形界面，   50%
    新增加可输出被略过的行数    OK
    错误抛出系统，可以将出错的行略过或者显示在图形界面   50%
    生成format_input对象都打印在Gui中
    info_Pro里 修改行数序号，与原Excel表一致 ok
    删除GetExcelInfo里关于Docx相关的内容，以后outputDocx要对传入G.output数据进行处理  50%






github 命令
`
git push -u origin master
`
打包命令
`
pyinstaller -F gui_creator.py
pyinstaller -F gui_c.2.py
pyinstaller -F -w check_box.py
`

#### 错误代码
    001  excel表转换异常
    002  参数获取错误
    003  以号代图未收录
    004  内容获取异常