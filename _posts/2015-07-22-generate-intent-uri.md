---
layout: blog
published: false
---

## AndroidインテントURIのについて

Androidでは、特定のリンクをブラウザ上から開く事で、媒介となるアプリも介さずに、ウェブページから指定のインテントを発する事ができます。

この方法でのインテントの送信には、ブラウザ上のAPIなどを介さず、intentスキームを持つURI(intent://..)のリンクを生成し、ユーザーに開いてもらうか、あるいはスクリプトで直接移動させる必要が有ります。
 
この時、単純なVIEWなどのアクションだけなら、生成は難しくないのですが、Parcelを介したパラメタ(Extraデータ)送信のための記述が不明瞭です。そこで、分解、及び生成のモジュールを探索してみました。

Enter text in [Markdown](http://daringfireball.net/projects/markdown/). Use the toolbar above, or click the **?** button for formatting help.