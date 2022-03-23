### hugo+bash=hush!

#### 配置文件示例
如果你正在配置一个全新的 hugo 站点，那么你可以直接用下面的配置覆盖 `config.toml` 中的内容。
```toml
baseURL = "https://jingyu.red/"
languageCode = "zh-Hans"
title = "鲸宇"
# 网站标题
theme = "hush"

[menu]
    [[menu.main]]
    identifier = "wenzhang"
    name = "文章"
    url = "/wenzhang/"
    weight = 1 

    [[menu.main]]
    identifier = "riji"
    name = "日记"
    url = "/riji/"
    weight = 2 

    [[menu.main]]
    identifier = "guanyu"
    name = "关于"
    url = "/guanyu/"
    weight = 3 
  
    [[menu.main]]
    identifier = "youlian"
    name = "友链"
    url = "/youlian/"
    weight = 4 

[markup]
    [markup.highlight]
    anchorLineNos = false
    codeFences = true
    guessSyntax = true
    lineNos = false
    lineNumbersInTable = false
    noClasses = true
    noHl = false
    style = 'manni'
    # manni 是我挑选的符合 hush 风格的主题。
    # 你也可以自己选择你喜欢的 Chroma 主题。
    # 点击下方网站查看主题列表。
    # https://xyproto.github.io/splash/docs/all.html
    tabWidth = 4

[params]
author = "Jingyu"
email = "example@example.org"
description = "我是站点描述。"
show = "wenzhang"
# 在这里填入你想要在首页展示的目录。
# 例如你想要展示 content 中 post 文件夹下的所有文章，
# 那你就应该在这里填 post 。

    [params.analytics]
        enable = "false"
        tid = "UA-XXXXXX-Y"
        api = "https://example.org/"
    # hush 默认使用 cfga 引入 Google Analytics 。
    # 查看这篇文章来了解如何填写 tid 和 api。
    # https://jingyu.red/wenzhang/zai-hugo-zhong-yibu-jiazai-google-analytics/

    [params.icon]
        url = "https://example.org/xxx.png"
        size = "16x16"
    # 在这里填写网站图标的链接，
    # 以及图标的分辨率。
```