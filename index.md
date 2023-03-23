---
layout: default
title: "yank.nvim"
---

## yank.nvim
ぼくだよ

<div class="quote-container">
	<p id="quote"></p>
	<p id="quote-from"></p>
	<button class="quote-reload" onclick="updateQuote()"><img src="assets/img/reload.png" height=16></button>
</div>
<a class="twitter-timeline" data-width="350" data-height="300" data-theme="light" href="https://twitter.com/yanknvim?ref_src=twsrc%5Etfw">Tweets by yanknvim</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

<script>
const quote = document.getElementById("quote");
const quote_from = document.getElementById("quote-from");

let quote_list = ["ケーキがなくなるまで、ひたすら試し続けるの です。", "捌いてみろ！2356ビーム！", "撃ちまくって強行突破する", "Curse of justice you don't know", "貴様の知己、貴様の愛した者、その全てとともに死ね", "君ビートマニア上手いねえ", "電気止まっちゃった"];
let quote_from_list = ["Still Alive / Portal", "音弾超人ゴリライザー / ゴリライザー製作委員会", "マスターチーフ / Halo 3", "void(Mournfinale) / Tesitfy", "ディアブロ / Diablo 3", "ギャラリー界 / beatmaniaIIDX", "クーネル・エンゲイザー / 電ǂ鯨"]

function updateQuote() {
	var index = Math.floor(Math.random() * quote_list.length);
	quote.textContent = quote_list[index];
	quote_from.textContent = quote_from_list[index];
}

updateQuote()
</script>
