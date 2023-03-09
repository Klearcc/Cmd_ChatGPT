# Cmd_ChatGPT
终端内快捷使用ChatGPT

## 效果

![image-20230309170642968](https://cdn.jsdelivr.net/gh/klearcc/pic/img202303091706999.png)

## 介绍

* 同一个问题，返回两次结果，可用来做对比。因为ChatGPT一本正经说瞎话可是出了名的。所以建议用两个token，py脚本内本人用了两个token。
* 请求耗时取决于自己的代理，py脚本内用的是http代理，端口为1087，可自行修改。
* 另外本人各个参数设置得比较高，问题的回答随机性较大。若使用不舒服建议自己设置各参数，脚本内有说明。

## 使用方式

1. 安装所需依赖

    ```
    pip install -r requirements.txt
    ```

    

2. 在[这里](https://platform.openai.com/account/api-keys)申请两个token，分别填入脚本内token1、token2

3. 添加下面内容至~/.bash_profile，xxxxx为脚本的绝对路径。保存后新建终端就可以使用了。

    ```
    #chatGPT cmd
    alias q="python xxxxx/cmd_ChatGPT.py -q "
    alias 去="python xxxxx/cmd_ChatGPT.py -q "
    ```

4. 终端内使用

    ```
    ###个人觉得Q键在左手边比较容易按
    q  你叫什么名字 谁给你取的呢
    ###或者
    去 你叫什么名字 谁给你取的呢
    ```
    
### 友情提示: 
    任何问题(包括有空格的问题)都可以直接输入终端；但当需要问有回车换行的内容(比如代码块)需要使用三引号包裹代码块
    <img width="1073" alt="image" src="https://user-images.githubusercontent.com/111847318/224000019-e622daee-5f63-4a69-a173-a21238ac5468.png">
    <img width="1071" alt="image" src="https://user-images.githubusercontent.com/111847318/224000550-d90dec07-3b52-43e0-8b35-5d4314f34b82.png">

    
    

    
