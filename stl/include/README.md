﻿# &lt;stl:include&gt; 包含文件

```html
<stl:include file="文件路径"></stl:include>
```

## 说明

通过 stl:include 标签在模板中包含另一个文件，作为模板的一部分。

通常此标签在处理诸如页头、页脚、版权声明等每个页面相同的内容时使用。

被 &lt;stl:include&gt; 标签包含的文件中可以包含其他 STL 标签或实体。

stl:include 类似于动态页面中的 <%@ include file="header.jsp" %>包含。
file是需要包含的文件名，一般以"~"或者"@"开头，代表系统根目录或站点目录下的文件，如 file="@/include/head.html"，也可以采用 file="/include/head.html"。

stl:include 标签能够解析包含文件中的 STL 标签或实体。
包含文件可以到"展示管理"—"包含文件管理"中管理。

&lt;stl:include&gt; 标签对应的实体为{stl:include}。

## 属性

| 属性                               | 说明     |
| ---------------------------------- | -------- |
| [file](include/attributes?id=file) | 文件路径 |