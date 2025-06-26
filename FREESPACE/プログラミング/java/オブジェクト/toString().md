2025-06-26
[[#Java]]
[[Java]]

---
## 🔷 `toString()`とは？

> `toString()` は、「オブジェクトを**文字列に変換するためのメソッド**」です。

Javaのすべてのクラスは、暗黙的に `Object` クラスを親にもっていて、  
その `Object` クラスに最初から `toString()` メソッドが定義されています。

✅ 例：toString()の使われ方

<div style="
  border: 2px solid blue;
  background-color: white;
  padding: 10px; 
  border-radius: 8px 8px 0px 8px;
  color: black;
  font-family: monospace;
  white-space: pre;
">
<pre><code>
String text = "こんにちは";
System.out.println(text); 
</code></pre>
</div>

実はこのとき、**Javaの中ではこう書いたのと同じことが起きています：**

<div style="
  border: 2px solid blue;
  background-color: white;
  padding: 10px; 
  border-radius: 8px 8px 0px 8px;
  color: black;
  font-family: monospace;
  white-space: pre;
">
<pre><code>System.out.println(text.toString());

</code></pre>
</div>

つまり、

- `System.out.println()` にオブジェクトを渡すと
    
- 自動で `toString()` を呼び出して
    
- そのオブジェクトを「人間が読める文字列」に変換して表示します。

