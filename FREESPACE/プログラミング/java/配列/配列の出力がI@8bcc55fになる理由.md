2025-06-26
[[#Java]]

---
<div style="
  border: 2px solid blue;
  background-color: white;
  padding: 10px; 
  border-radius: 8px 8px 0px 8px;
  color: black;
  font-family: monospace;
  white-space: pre;
">
<pre><code>public class array{
    public static void main(String[] args){
        int[] score = new int[5];
        score[3] = 34;
        System.out.println(score.length);
        System.out.println(score);
        
    }
}</code></pre>
</div>

   =>5
   =>[I@8bcc55f

1. 配列はオブジェクトである
	`int[] score = new int[5];` は、長さ5のint型配列[[オブジェクト]]を作っている。
	
2. System.out.println(score) は何をしているか
	System.out.println(オブジェクト) は、オブジェクトの[[toString()]]メソッドを呼び出す。
3.  配列のtoString()の中身
	配列（int[]）はObjectクラスから継承されるtoString()をそのまま使うので、以下の形式で出力されます
	<div style="
  border: 2px solid blue;
  background-color: white;
  padding: 10px; 
  border-radius: 8px 8px 0px 8px;
  color: black;
  font-family: monospace;
  white-space: pre;
">
<pre><code>[型情報@ハッシュ値（16進数）]</code></pre>
</div>

| 項目         | 値                           |
| ---------- | --------------------------- |
| `[`        | 配列であることを表す                  |
| `I`        | 配列の要素がint型であることを表す（I = int） |
| `@8bcc55f` | オブジェクトのハッシュコード（16進数）        |