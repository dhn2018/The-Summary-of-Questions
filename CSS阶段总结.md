<font size='4'>

# white-space

1. 设置如何处理元素中的空白
2. 所有浏览器均支持，但均不支持其inherit属性
3. 属性值如下：

    ----- | 换行符	| 空格和制表符 | 文字转行
    ----- | ----- | ----- | -----
    normal | 合并 | 合并 | 转行
    nowrap | 合并 | 合并 | 不转行
    pre | 保留 | 保留 | 不转行
    pre-wrap | 保留 | 保留 | 转行
    pre-line | 保留 | 合并 | 转行

# word-break

-  设置怎么在单词内断行
    1.  normal: 使用默认的断行规则 
    2.  break-all：单词任意位置断行 
    3.  keep-all： 单词不断行 

## 文本两端对齐

- 文本对齐方式text-align定义行内内容如何相对于它的块级父元素对齐， 
__不是设置块元素本身对齐__

> __常用__：    
left：居左  
right： 居右  
center： 居中  
justify：两端对齐（除最后一行）  
justify-all：两端对齐（强制最后一行也对齐）  
__实验性API__：    
start: 内容为从左至右时，同left  
end： 内容为从左至右时，同right  
<string>: 第一个出现的该字符串被用来对齐

- 两端对齐

    justify最后一行没有效果：
    - 最后一行或只有一行：text-align-last: justify; （但是这个属性并不是所有浏览器都支持）
    - 手动添加最后一行并隐藏：（即为把最后一行变为不是最后一行）
    ```
    .box {
        width: 200px;
        text-align: justify;
    }
    .box:after {   // 利用伪类
        content: '';
        display: inline-block;
        width: 100%;     // 设置足够宽，确保它占了最后一行
    }
    ```
    __注意：__ 后面加空行也没有效果，必须是空元素！

# line-height
行高有4种设置方式：
- 数字：line-height:1; 表示行中文本高度的倍数，同line-height:1em;
- 长度：line-height:20px; 直接设置
- 百分比：line-height: 150%; 
- 关键字：line-height:normal; 还有inherit、initial、unset，默认值normal取决于用户端、浏览器，约为1.2

## 一个按钮的实现方式
1. <imput type="button"/> 这就是一个按钮，但是点击没有回调
2. <imput type="submit"/> 放在form表单中相当于提交按钮，点击提交表单
3. button按钮             同2，放在form表单中点击提交表单，不同之处是它还可以包含图片等多媒体内容
4. img、div、a、span等其他标签改装
4种方式均为原生，都可以加背景
    


</font>
