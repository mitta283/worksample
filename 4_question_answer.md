>Railsにおける、「単数」と「複数」の使い分けについての説明です。

>例えばコントローラー作成時は"blogs"と、モデル作成時は"blog”とそれぞれパラメーター指定させています。それに基づいて様々な変数等が自動的に作成されているようなので、"blogs"と"blog"を使い分けることに意味があるのだと思うのですが、何処にも記載が無いので未だに混乱しています。

>rake routes"を行ってみても、Prefixに"blog"　”new_blog"もあれば、"blogs" "confirm_blogs"もあります。何故こうなっているのか全く理解できていません。

ご質問ありがとうございます。

結論から言うとこれはRailsの定める規約に基づく命名で、モデルクラスは単数形、テーブルスキーマ、コントローラーは複数形と定められているためです。（参考：[Railsのサイト](https://guides.rubyonrails.org/)を見ていただき、各項の"Naming Convention"が命名規約に関する部分です。)

まず前提としてRailsはパフォーマンスにおいて悩むべきではないものについて設定ではなく規約として定めることで、開発効率を高めているツールです。
特にファイルやフォルダの命名はパフォーマンスには直接影響しませんから、私達が各々考えるよりも規約に沿って命名する方が効率がよいというのはご理解いただけるかと思います。

[当社のブログ](https://diveintocode.jp/blogs/Technology/NamingRole)でもご質問の多い項目であることから解説をさせていただいておりましたが、もしテキストのこの部分に補足があれば混乱しなかったのに、という箇所がございましたら差し支えなければお伝えいただけると今後の参考とさせていただきます。

また、回答に不足があればお気軽にお申し付けください。
