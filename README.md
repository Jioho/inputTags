# inputTags

#### 项目介绍
input输入标签插件

#### 参数说明
* @param elem                      (必填参数) 触发对象的id/class/tag
* @param content                   数据源,需要显示的数据
* @param inputType                 输入框类型
* @param theme                     标签背景颜色
* @param placeholder               input框的水印（提示文字）
* @param regular                   正则验证。不填写改参数这不开启验证
*        regular =>  rule          正则验证规则，支持自己输入表达式，或者使用内置验证（mobile手机、email邮箱、no_chinese非中文）
*        regular =>  err_callback  验证失败回调 （code 错误代码  msg 错误提示）
* @param beforeEnter               在回车之前判断的函数，可以使用return false阻止回车时间
* @param afterEnter                回车后的回调函数，返回当前框所有的值

____

#### 函数说明(实例化之后才可用)
* @function clearAll()       参数 无参                   清空输入框标签
* @function reload()         参数 一维数组               重新渲染输入框的标签，每次重新渲染都会清除旧数据
* @function getValue()       参数 无参                   获取输入框中的标签
* @function on()             参数 操作类型,回调方法       目前操作类型只有 delTag 再删除标签后的回调方法