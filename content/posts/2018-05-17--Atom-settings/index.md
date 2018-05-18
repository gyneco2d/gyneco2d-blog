---
title: Atomで拡張子ごとにシンタックスを指定する
subTitle: jsxファイルをjsシンタックス，jadをjavaシンタックスで開く
category: settings
cover: ../article_icons/settings.jpg
---

`Atom > Config...`で以下を開く

`config.cson`
```coffeescript
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
```

`.jsx`ファイルがJavaScript，`.jad`ファイルがJavaとして開くようになる．
