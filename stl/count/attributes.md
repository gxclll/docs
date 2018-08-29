# &lt;stl:acount&gt; 属性

下表显示所有属于此标签的属性列表。

## type

显示类型：

- `"Channels"` 统计栏目数
- `"Contents"` 统计内容数
- `"Comments"` 统计评论数
- `"Downloads"` 统计下载次数、下载量

## channelIndex

栏目索引

## channelName

栏目名称

## upLevel

指定统计上几级栏目的数据，0 为本级，1 为父栏目，以此类推。

## topLevel

指定统计从首页向下某个级别栏目的数据，0 代表网站首页，1 代表一级栏目，以此类推。

## scope

统计范围。此属性只可属于以下可能的取值的一种。

- `"Self"` 仅统计当前栏目或内容下的数据
- `"Children"` 统计下级栏目的数据
- `"SelfAndChildren"` 统计本级栏目及下一极子栏目下的数据
- `"Descendant"` 统计所有级别的子栏目下的数据
- `"All"` 统计所有栏目的数据

## since

时间段，格式为"数字+日期符号"，日期符号有"y"、"m"、"d"及"h"，分别代表年、月、天及小时。