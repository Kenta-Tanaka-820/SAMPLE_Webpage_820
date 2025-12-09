# SAMPLE_Webpage_820

# Webページ制作作品（HTML/CSS/JavaScript）

## 概要
この作品は、大学の授業課題として制作したシンプルなWebページです。
Webの基本的な構造を理解することを目的とし、複数ページ構成、スタイル設定、JavaScriptによる動的処理を取り入れています。

---

## 使用技術
- HTML
- CSS（外部スタイルシート）
- JavaScript（DOM操作・イベント処理）

---

## ページ構成
- `index.html`：トップページ
- `about.html`：アルバム紹介ページ
- `prof.html`：メンバー紹介ページ

ページ遷移はヘッダーナビゲーションから行えるように設計しています。

---

## 実装ポイント / 工夫した点

- `header`・`nav`・`section`などのセマンティックHTMLを意識してマークアップしました。
- CSSを外部ファイルとして分離し、HTML構造とスタイルを整理しました。
- JavaScriptでボタン操作に応じてページ内テキストを書き換える機能を実装し、静的なページだけでなく簡単な動的挙動も含めています。

```javascript
var element = document.getElementById("info");
var button = document.getElementById("change");
button.addEventListener("click", function() {
    element.innerHTML = "kinggnuホームページ(https://kinggnu.jp/)をご覧ください";
});


