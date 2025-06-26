2025-06-07
[[#Java]]
[[Java]]


---
- ファイル名の後につづく文字は実行時にそのプログラムに渡される文字列（引数）**引数**になる


<div style="
  border: 2px solid blue;
  background-color: white;
  padding: 10px; 
  border-radius: 8px 8px 0px 8px;
  color: black;
  font-family: monospace;
  white-space: pre;
">
<pre><code>public class Sample {
    public static void main(String[] args) {
        System.out.println("1番目の引数：" + args[0]);
        System.out.println("2番目の引数：" + args[1]);
    }
}</code></pre>
</div>

→
1番目の引数：5
2番目の引数：2

- もし数値として使いたければ、`Integer.parseInt(args[0])` のように変換する

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
public class Sample {
    public static void main(String[] args) {
        int a = Integer.parseInt(args[0]);
        int b = Integer.parseInt(args[1]);
        System.out.println("合計：" + (a + b));
    }
}</code></pre>
</div>

→
合計：7



