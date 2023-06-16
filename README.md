# HTML-7-
HTML的表格、列表、块
//HTML表格
    <html>

    <body>

    <p>每个表格由table标签开始</p>
    <p>每个表格行由tr标签开始</p>
    <p>每个表格数据由td标签开始</p>

    <h4>一列：</h4>
    <table border="1">
    </tr>
    </table>

    <h4>一行三列：</h4>
    <table border="1">
    <tr>
      <td>100</td>
      <td>200</td>
      <td>300</td>
    </tr>
    </table>

    <h4>两行三列：</h4>
    <table border="1">
    <tr>
      <td>100</td>
      <td>200</td>
      <td>300</td>
    </tr>
    <tr>
      <td>400</td>
      <td>500</td>
      <td>600</td>
      </tr>
      </table>

      </body>
      </html>
      //注：其中的border可以改数值来调节边框的厚度
      //字母td指表格数据，即数据单元格的内容。数据单元格包含文本、图片、列表、段落、表单、水平线、表格等

      //表格的边框与属性
      //如果不定义边框属性，表格将不显示边框

      //表格的表头
      //表格的表头使用<th>标签进行定义
      //大多数浏览器会把表头显示为粗体居中的文本
      <table border="1">
      <tr>
      <th>Heading</th>
      <th>Another Heading</th>
      </tr>
      <tr>
      <td>row 1,cell 1</td>
      <td>row 1,cell 2</td>
      </tr>
      <tr>
      <td>row 2,cell 1</td>
      <td>row 2,cell 2</td>
      </tr>
      </table>
      //一般这里的th是会加粗居中的，这里还用了<tr>括了起来

      //表格中的空单元格
      //在一些浏览器中，没有内容的表格单元显得不太好，如果表格单元没有内容，浏览器则无法显示出这个单元格的边框
      //为了解决这个问题，在空单元格中添加一个空格占位符，就可以显示边框了
      <table border="1">
      <tr>
      <td>row 1,cell 1</td>
      <td>row 1,cell 2</td>
      </tr>
      <tr>
      <td>&nbsp;</td>
      <td>row 2,cell 2</td>
      </tr>
      </table>

      //表格需要带标题用<caption>标签
      <caption>我的标题</caption>

      //跨两行单元格与跨两列单元格
      <th colspan="2">电话</th>
      <th>rowspan="2">电话</th>

      //单元格边距(cell padding),单元格内部的范围更加大一些
      <h4>带有cellpadding：</h4>
      <table border="1"
      cellpadding="10">
      <tr>
        <td>First</td>
        <td>Row</td>
      </tr>
      <tr>
        <td>Second</td>
        <td>Row</td>
      </tr>
      </table>

      </body>
      </html>

      //单元格间距(cellspacing):边框更加大
      <h4>带有cellspacing:</h4>
      <table border="1"
      ce;;spacing="10">
      <tr>
        <td>First</td>
        <td>Row</td>
      </tr>
      <tr>
        <td>Second</td>
        <td>Row</td>
      </tr>
      </table>

      </body>
      </html>

      //向表格添加背景颜色或背景图像
      <table border="1"
      bgcolor="red">
      //背景图像
      <table border="1"
      background="/i/eg_bg_07.gif">

      //向单元格添加背景颜色和背景图像
      //在<td>里面添加样式
      <tr>
        <td bgcolor="red">First</td>
        <td>Row</td>
      </tr>
      //图像同理

      //在表格单元中排列内容
      <html>

      <body>

      <table width="400" border="1">
      <tr>
        <th align="left">消费项目。。。</th>
        <th align="right">一月</th>
        <th align="right">二月</th>
      </tr>
      </table>

      //框架属性
      //在table中定义
      <table frame="box">
      <table frame="above">
      //等等

      //标签积累：
      <table>//定义表格
      <caption>//定义表格标题
      <th>//定义表格表头
      <tr>//定义表格行
      <td>//定义表格单元
      <thead>//定义表格页眉
      <tbody>//定义表格的主体
      <tfool>//定义表格的页脚
      <col>//定义用于表格列的属性
      <colgroup>//定义表格列的组

//HTML列表
    //HTML支持有序、无序和定义列表
    <html>

    <body>

    <h4>一个无序列表：</h4>
    <ul>
      <li>咖啡</li>
      <li>茶</li>
      <li>牛奶</li>
    </ul>

    </body>
    </html>

    //有序列表
    <html>
    <body>

    <ol>
      <li>咖啡</li>
      <li>牛奶</li>
      <li>茶</li>
    </ol>

    <ol start="50">
      <li>咖啡</li>
      <li>牛奶</li>
      <li>茶</li>
    </ol>

    </body>
    </html>

    //无序列表
    //无序列表是一个项目的列表，此项目使用粗体圆点(典型的小黑圆圈)进行标记
    //无序标签<ul>标签。每个列表项始于<li>
    <ul>
    <li>Coffee</li>
    <li>Milk</li>
    </ul>
    //列表内部可以使用段落、换行符、图片、链接以及其他列表等等

    //有序列表
    //有序列表始于<ol>标签，每个列表项始于<li>标签
    <ol>
    <li>Coffee</li>
    <li>Milk</li>
    </ol>

    //定义列表、
    //自定义列表不仅仅是一列项目，而是项目及其注释的组合
    //自定义列表以<dl>标签开始，每个自定义列表项以<dt>开始，每个自定义列表项的定义以<dd>开始
    <dl>
    <dt>Coffee</dt>
    <dd>Black hot drink</dd>
    <dt>Milk>/dt>
    <dd>White cold drink</dd>
    </dl>
    //列表内部可以使用段落、换行符、图片、链接以及其他列表等等

    //不同类型的无序列表
    <html>
    <body>

    <h4>Disc 项目符号列表：</h4>
    <ul type="disc">
      <li>苹果</li>
      <li>香蕉</li>
      <li>柠檬</li>
      <li>桔子</li>
    </ul>
    //<ul type>这个类型还有circle，square等

    //不同类型的有序列表
    <html>
    ,body>

    <h4>数字列表</h4>
    <ol>
      <li>苹果</li>
      <li>香蕉</li>
      <li>柠檬</li>
      <li>桔子</li>
    </ol>
    //在这里<ol>标签的type的类型可以定义为"A"、"a"、"I"、"i".(后面两个为罗马数字)

    //嵌套列表
    <html>

    <body>

    <h4>一个嵌套列表：</h4>
    <ul>
      <li>咖啡</li>
      <li>茶
        <ul>
        <li>红茶</li>
        <li>绿茶</li>
        </ul>
      </li>
      <li>牛奶</li>
    </ul>

    </body>
    </html>

    //定义列表
    <html>

    <body>

    <h2>一个定义列表：</h2>

    <dl>
      <dt>计算机</dt>
      <dd>用来计算的仪器......</dd>
      <dt>显示器</dt>
      <dd>以视觉方式显示信息的装置......</dd>
    </dl>

    </body>
    </html>

    //标签积累：
    <ol>//定义有序列表
    <ul>//定义无序列表
    <li>//定义列表项
    <dl>//定义定义列表
    <dt>//定义定义项目
    <dd>//定义定义的描述
    <dir>//已废弃，使用<ul>代替它
    <menu>//已废弃，使用<ul>代替它

//HTML块
    //可以通过<div>和<span>将HTML元素组合起来

    //HTML块元素
    //大多数HTML元素被定义为块级元素或内联元素
    //块级元素在浏览器显示时，通常会以新行来开始和结束
    //例；<h1>,<p>,<ul>,<table>

    //HTML内联元素
    //内联元素在显示时通常不会以新行开始
    //例：<b>,<td>,<a>,<img>

    //HTML<div>元素
    //HTML<div>元素是块级元素，可用于组合其他HTML元素的容器
    //<div>元素没有特定的含义，由于它属于块级元素，浏览器会在其前后显示折行
    //如果与CSS同时使用<div>元素可用于对大的内容块设置样式属性
    //<div>的另一个常见用途是文档布局。它取代了表格定义布局的老式方法。用<table>也不是表格的正确使用方法<table>元素是显示表格式化的数据

    //HTML<span>元素
    //HTML<span>元素是内联元素，可用作文本的容器
    //<span>元素也没有特定的含义
    //当与CSS一同使用时，<span>元素可用于为部分文本设置样式属性

    //标签积累：
    <div>//定义文档中的分区或节
    <span>//定义span，用来组合文档中的行内元素
