---
title: jekyll now yaml
date: 2015-11-09
tags: ["jekyll", "markdown"]
---

``jekyll-now``を使い始めて色々と調べていますが、一時的なのだけれど記録を残します。

どうやら、``posts``するファイルはマークダウン方式を使っているのだけれど、その``Head``の部分でトラブル発生

<!--more-->

```yaml
---
layout:
- post
title:
- jekyll now yaml
---
```


ではなく、以下のようでなくてはいけません。

{% highlight yaml linenos %}
---
layout: post
title: jekyll now yaml
---
{% endhighlight %}

仕様にもこのような記述になっていました。
カテゴリーなどの部分ではどうなるのか？
