# _archive

もとの個人ポータル一式の退避場所。

- `site-v1/` … 2026-07 まで公開していたポータル（index.html / style.css / 画像類）そのまま。

GitHub Pages（Jekyll）は `_` で始まるディレクトリを配信しないため、
ここに置いてある間は `warpshoot.github.io/_archive/...` にアクセスしても表示されません。
（リポジトリ自体が public の場合、GitHub 上ではファイルとして見えます）

## 元に戻すには

リポジトリのルートで:

```sh
git rm index.html                      # プレースホルダーを削除
git mv _archive/site-v1/* .            # 退避したファイルを戻す
git commit -m "Restore portal"
git push
```

favicon.png はルートに残してあるので、戻すときに上書きしてもしなくても同じです。
