## coe记录 蔡蔡

#### dayone：sublime工具和html标签的使用
[sublime插件的竞技场](https://docs.google.com/presentation/d/1i9XqxfIX4oDNYMa5DlfLJChHnl3iR44OdKjIG6TCHoI/edit#slide=id.g1a8f551ac1_0_0)

#### daytwo: css中的常见问题  孙孙
[nodePPT](https://github.com/ksky521/nodePPT)

###### 酷炫的分享ppt形式，前提是安装nodejs 

[nodejs安装教程](http://jingyan.baidu.com/article/b0b63dbfca599a4a483070a5.html)
[nodejs官网](https://nodejs.org/en/)_

###### 自己安装教程，node.js搞定了，然后怎么用npm安装其他东西呢？

*1* 首先，win+R ，cmd，开启一个命令行窗口
    
    Microsoft Windows [版本 10.0.14393]
    (c) 2016 Microsoft Corporation。保留所有权利。

*2* 输入node 

        C:\Users\user>node
    > 

*3* 如果你天真的以为接下来是直接在> 后面输入nmp 安装命令，那么你就sb啦！

    C:\Users\user>node
    > nmp install -g nodeppt
    nmp install -g nodeppt
        ^^^^^^^
    SyntaxError: Unexpected identifier

    //姐姐我不服！
    > sudo nmp install -g nodeppt
    sudo nmp install -g nodeppt
    SyntaxError: Unexpected identifier

    //越挫越勇
    > npm install -g nodeppt
    npm should be run outside of the node repl, in your normal shell.
    //哈哈，终于报了一个可以百度的错误了……

*4* [这位小伙和我演了类似的情景剧](http://blog.csdn.net/davislien/article/details/46858511)
    
######解释： 这个提示中的“repl”指的是node自己提供的那个控制台环境（就是我们刚才一直输入信息的控制台），其中可以进行运算操作，也就是直接输入js语句，但不能输入命令。理解为环境比较好！

######解决方案： win+R cmd 开启一个新的命名行窗口
    npm install -g nodeppt


    C:\Users\user\AppData\Roaming\npm\nodeppt -> C:\Users\user\AppData\Roaming\npm\node_modules\nodeppt\bin\nodeppt

    > ws@0.4.31 install C:\Users\user\AppData\Roaming\npm\node_modules\nodeppt\node_modules\engine.io-client\node_modules\ws
    > (node-gyp rebuild 2> builderror.log) || (exit 0)


    C:\Users\user\AppData\Roaming\npm\node_modules\nodeppt\node_modules\engine.io-client\node_modules\ws>if not defined npm_config_node_gyp (node "D:\Program Files\node.js\node_modules\npm\bin\node-gyp-bin\\..\..\node_modules\node-gyp\bin\node-gyp.js" rebuild )  else (node "" rebuild )

    > ws@0.5.0 install C:\Users\user\AppData\Roaming\npm\node_modules\nodeppt\node_modules\ws
    > (node-gyp rebuild 2> builderror.log) || (exit 0)


    C:\Users\user\AppData\Roaming\npm\node_modules\nodeppt\node_modules\ws>if not defined npm_config_node_gyp (node "D:\Program Files\node.js\node_modules\npm\bin\node-gyp-bin\\..\..\node_modules\node-gyp\bin\node-gyp.js" rebuild )  else (node "" rebuild )
    C:\Users\user\AppData\Roaming\npm
    `-- nodeppt@1.4.2
      +-- chokidar@1.6.1
      | +-- anymatch@1.3.0
      | | +-- arrify@1.0.1
      | | `-- micromatch@2.3.11
      | |   +-- arr-diff@2.0.0
      | |   | `-- arr-flatten@1.0.1
      | |   +-- array-unique@0.2.1
      | |   +-- braces@1.8.5
      | |   | +-- expand-range@1.8.2
      | |   | | `-- fill-range@2.2.3
      | |   | |   +-- is-number@2.1.0
      | |   | |   +-- isobject@2.1.0
      | |   | |   +-- randomatic@1.1.6
      | |   | |   `-- repeat-string@1.6.1
      | |   | +-- preserve@0.2.0
      | |   | `-- repeat-element@1.1.2
      | |   +-- expand-brackets@0.1.5
      | |   | `-- is-posix-bracket@0.1.1
      | |   +-- extglob@0.3.2
      | |   +-- filename-regex@2.0.0
      | |   +-- kind-of@3.1.0
      | |   | `-- is-buffer@1.1.4
      | |   +-- normalize-path@2.0.1
      | |   +-- object.omit@2.0.1
      | |   | +-- for-own@0.1.4
      | |   | | `-- for-in@0.1.6
      | |   | `-- is-extendable@0.1.1
      | |   +-- parse-glob@3.0.4
      | |   | +-- glob-base@0.3.0
      | |   | `-- is-dotfile@1.0.2
      | |   `-- regex-cache@0.4.3
      | |     +-- is-equal-shallow@0.1.3
      | |     `-- is-primitive@2.0.0
      | +-- async-each@1.0.1
      | +-- glob-parent@2.0.0
      | +-- inherits@2.0.3
      | +-- is-binary-path@1.0.1
      | | `-- binary-extensions@1.8.0
      | +-- is-glob@2.0.1
      | | `-- is-extglob@1.0.0
      | +-- path-is-absolute@1.0.1
      | `-- readdirp@2.1.0
      |   +-- graceful-fs@4.1.11
      |   +-- minimatch@3.0.3
      |   | `-- brace-expansion@1.1.6
      |   |   +-- balanced-match@0.4.2
      |   |   `-- concat-map@0.0.1
      |   +-- readable-stream@2.2.2
      |   | +-- buffer-shims@1.0.0
      |   | +-- core-util-is@1.0.2
      |   | +-- isarray@1.0.0
      |   | +-- process-nextick-args@1.0.7
      |   | +-- string_decoder@0.10.31
      |   | `-- util-deprecate@1.0.2
      |   `-- set-immediate-shim@1.0.1
      +-- colors@1.1.2
      +-- commander@2.9.0
      | `-- graceful-readlink@1.0.1
      +-- connect@2.11.0
      | +-- buffer-crc32@0.2.1
      | +-- bytes@0.2.1
      | +-- cookie@0.1.0
      | +-- cookie-signature@1.0.1
      | +-- fresh@0.2.0
      | +-- methods@0.0.1
      | +-- multiparty@2.2.0
      | | +-- readable-stream@1.1.14
      | | | `-- isarray@0.0.1
      | | `-- stream-counter@0.2.0
      | |   `-- readable-stream@1.1.14
      | |     `-- isarray@0.0.1
      | +-- negotiator@0.3.0
      | +-- pause@0.0.1
      | +-- qs@0.6.5
      | +-- raw-body@0.0.3
      | +-- send@0.1.4
      | | +-- mime@1.2.11
      | | `-- range-parser@0.0.4
      | `-- uid2@0.0.3
      +-- cookie@0.2.4
      +-- debug@2.3.3
      | `-- ms@0.7.2
      +-- ejs@0.8.4
      +-- ipv4@0.0.4
      +-- mathjax@2.6.1
      +-- read@1.0.7
      | `-- mute-stream@0.0.6
      `-- socket.io@1.3.3
        +-- debug@2.1.0
        | `-- ms@0.6.2
        +-- engine.io@1.5.1
        | +-- base64id@0.1.0
        | +-- debug@1.0.3
        | | `-- ms@0.6.2
        | +-- engine.io-parser@1.2.1
        | | +-- after@0.8.1
        | | +-- arraybuffer.slice@0.0.6
        | | +-- base64-arraybuffer@0.1.2
        | | +-- blob@0.0.2
        | | +-- has-binary@0.1.5
        | | | `-- isarray@0.0.1
        | | `-- utf8@2.0.0
        | `-- ws@0.5.0
        |   +-- nan@1.4.3
        |   +-- options@0.0.6
        |   `-- ultron@1.0.2
        +-- has-binary-data@0.1.3
        | `-- isarray@0.0.1
        +-- socket.io-adapter@0.3.1
        | +-- debug@1.0.2
        | | `-- ms@0.6.2
        | +-- object-keys@1.0.1
        | `-- socket.io-parser@2.2.2
        |   +-- debug@0.7.4
        |   `-- isarray@0.0.1
        +-- socket.io-client@1.3.3
        | +-- backo2@1.0.2
        | +-- component-bind@1.0.0
        | +-- component-emitter@1.1.2
        | +-- debug@0.7.4
        | +-- engine.io-client@1.5.1
        | | +-- component-inherit@0.0.3
        | | +-- debug@1.0.4
        | | | `-- ms@0.6.2
        | | +-- has-cors@1.0.3
        | | | `-- global@2.0.1
        | | +-- parsejson@0.0.1
        | | +-- parseqs@0.0.2
        | | +-- parseuri@0.0.4
        | | +-- ws@0.4.31
        | | | +-- commander@0.6.1
        | | | +-- nan@0.3.2
        | | | `-- tinycolor@0.0.1
        | | `-- xmlhttprequest@1.5.0
        | +-- has-binary@0.1.6
        | | `-- isarray@0.0.1
        | +-- indexof@0.0.1
        | +-- object-component@0.0.3
        | +-- parseuri@0.0.2
        | | `-- better-assert@1.0.2
        | |   `-- callsite@1.0.0
        | `-- to-array@0.1.3
        `-- socket.io-parser@2.2.3
          +-- benchmark@1.0.0
          +-- debug@0.7.4
          +-- isarray@0.0.1
          `-- json3@3.2.6

    npm WARN optional SKIPPING OPTIONAL DEPENDENCY: fsevents@^1.0.0 (node_modules\nodeppt\node_modules\chokidar\node_modules\fsevents):
    npm WARN notsup SKIPPING OPTIONAL DEPENDENCY: Unsupported platform for fsevents@1.0.15: wanted {"os":"darwin","arch":"any"} (current: {"os":"win32","arch":"x64"})

###### 成功啦！ppt的效果好赞啊！学习学习！
###### 滚去实现雷雨发庄稼啦！