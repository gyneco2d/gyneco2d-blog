---
title: Atomで拡張子ごとにシンタックスを指定する
subTitle: jsxファイルをjsシンタックス，jadをjavaシンタックスで開く
category: settings
cover: settings.jpg
---

`Atom > Config...`で以下を開く

`config.cson`
```CoffeeScript
"*":
  core:
    # 追記 -----------------
    customFileTypes:
        "source.js": [
            "jsx"
        ]
        "source.java": [
            "jad"
        ]
    # ----------------------
    telemetryConsent: "limited"
  editor:
    tabLength: 4
  "exception-reporting":
    userId: "889160bf-e2e3-466e-8f04-437dcde66029"
  welcome:
    showOnStartup: false
```

`.jsx`ファイルがJavaScript，`.jad`ファイルがJavaとして開くようになる．
