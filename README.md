我在写 iOS 的快捷指令（shortcuts）的时候需要有个方法来判断是不是工作日……所以解决办法就成了这样了。

具体使用的时候：

1. 先格式化日期，日期格式自定，格式化字串

    'https://tiansh.github.io/gzr/'yyyy/M/d'.json'

2. 然后获取“格式化后的日期”内容
3. 最后匹配“URL的内容”中的“true”

节假日仅包含全国性节假日，不包含地区节假日。

----

Workdays in P.R.China; query `'https://tiansh.github.io/gzr/'yyyy/M/d'.json'`, response json will be `{"isWorkday":false}` or `{"isWorkday":true}`. Support year 2019-2025. Only national holidays are inclcuded.
