---
title: CSSStyleDeclaration.item()
slug: Web/API/CSSStyleDeclaration/item
tags:
- API
- CSSOM
- Method
- Reference
browser-compat: api.CSSStyleDeclaration.item
translation_of: Web/API/CSSStyleDeclaration/item
---
<p>{{ APIRef("CSSOM") }}</p>

<p id="Summary"><span class="seoSummary"><code>CSSStyleDeclaration.item()</code> メソッドインターフェイスは、位置を指定して {{domxref('CSSStyleDeclaration')}} の CSS プロパティ名を返します。</span>このメソッドは与えた値による例外が発生しません。位置が範囲外だった場合は空文字列が返され、引数が与えられなかった場合は <code>TypeError</code> が発生します。</p>

<h2 id="Syntax">構文</h2>

<pre class="brush: js">var <em>propertyName</em> = <em>style</em>.item(<em>index</em>);
</pre>

<h3 id="Parameters">引数</h3>

<ul>
  <li><em><code>index</code></em> は読み取るノードの位置です。位置は 0 から始まります。</li>
</ul>

<h3 id="Return_value">返値</h3>

<ul>
  <li><em><code>propertyName</code></em> は {{domxref('DOMString')}} で、指定された位置にある CSS プロパティの名前を返します。</li>
</ul>

<p>JavaScript には、 NodeList から位置を指定して項目を取得するための簡単な特別な構文があります。
</p>

<pre class="brush: js">var propertyName = style[index];
</pre>

<h2 id="Example">例</h2>

<pre class="brush: js">var style = document.getElementById('div1').style;
var propertyName = style.item(1); // または style[1] - リスト中の 2 番目のスタイルを返します</pre>

<h2 id="Specifications">仕様書</h2>

{{Specifications}}

<h2 id="Browser_compatibility">ブラウザーの互換性</h2>

<p>{{Compat}}</p>