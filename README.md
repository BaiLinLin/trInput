# trInput

> 实现了简单的表单验证，通过设置 input 元素的 tr-valid 属性的类型来确定表单验证的类型，目前实现的有，phone，url，email 三种类型

## 使用方式

1. 通过 ｀npm intsall trinput｀来将组建文件安装到你的项目中
2. 在你的项目中引入 jquery，因为我们的组建是依赖于 jquery 实现
3. 在你的项目里引入 bootstrap.css 文件，因为我们的基本样式是以 bootstrap 为规范，或者你也可以自定义样式
4. 为你的表单设置 tr-valid 属性值
5. 当你提交表单的时候你就能惊奇的发现，你能进行表单验证了


### html 示例

        <form action="" name="demoForm">
            <div>
                <span>email</span>
                <input type="text" placeholder="email" tr-valid="email">
            </div>
        
            <div>
                <span>请输入手机号</span>
                 <input type="text" placeholder="phone" tr-valid="phone">
            </div>

            <div>
                <span>请输入url</span>
                <input type="text" placeholder="url" tr-valid="url">
            </div>

            <button>提交</button>
         </form>


##  trInput 计划迭代版本

 v0.0.1 实现目标
 
       验证类型可配置
           1. email
           2. phone
           3. url
 
 v0.0.2 实现目标
 
       参数可配置
           1. require 是否必填
           2. minlength 最小长度
           3. maxlength 最大长度
           4. pattern 正则验证
           5. name 表单名称
           6. 对 input 和 radio ,checkbox 做个区别