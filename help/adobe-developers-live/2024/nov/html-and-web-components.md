---
title: Web コンポーネントを使用した独自のHTMLの実行
description: Adobeのシニアデベロッパーエバンジェリストである Raymond Camden を使用して、web コンポーネントの基本を学びます。これには、カスタムPDF、シャドウ DOM、HTMLテンプレートが含まれ、要素の埋め込みや並べ替え可能なテーブルの構築などの実践的な例があります。
topic: Development
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2580
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16579
source-git-commit: 8770c8172ee90524079efc65aec7e129f1d1d031
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---


# Web コンポーネントを使用した独自のHTMLの実行

Adobeのシニアデベロッパーエバンジェリスト、Raymond Camden が、カスタム要素、シャドウ DOM、HTMLテンプレートなど、web コンポーネントの基本について説明します。 PDFの埋め込みや並べ替え可能なテーブルの構築など、実際の例を確認し、再利用可能な最新のソリューションでアプリケーションを強化します。

>[!VIDEO](https://video.tv.adobe.com/v/3440406/?learn=on&enablevpops)

## コミュニティ ディスカッション

Adobe Developers Live コミュニティで会話を続けます [&#x200B; ディスカッション &#x200B;](https://adobe.ly/48PRE63)。

## 重要な留意点

* **Web コンポーネントの概要** Web コンポーネントを使用すると、デベロッパーは、JavaScriptを使用して定義された、独自の外観とインタラクティブ機能を持つカスタムHTML要素を作成できます。
* **コアテクノロジー** web コンポーネントは、カスタム要素**シャドウ DOM、HTMLテンプレートという 3 つのコアテクノロジーを使用して構築されます。
* **カスタム要素** カスタム要素を使用すると、新しいHTMLタグを作成できます。 ケバブケースとダッシュを使用する必要があります。 JavaScript クラスは、その動作を定義するために使用されます。
* **シャドウ DOM** シャドウ DOM は、コンポーネントの DOM ツリーのカプセル化を行い、CSS のリークを防ぎ、より詳細に制御されたスタイル設定を可能にします。
* **HTMLテンプレート** HTMLテンプレートを使用すると、複製して DOM に追加できるHTMLと CSS を定義できます。 ただし、プレゼンターは、テンプレートよりもスロットを使用した方が配布や柔軟性が向上します。
* **属性とイベント** カスタム要素には、connectedCallback や disconnectedCallback などの属性とイベントハンドラーを含め、DOM から追加または削除されたときの動作を管理できます。
* **スロット** スロットを使用すると、コンテンツを web コンポーネントに挿入でき、デフォルトスロットと名前付きスロットの両方をサポートして、より柔軟にコンテンツを管理できます。
* **実際の例** 例としては、PDF埋め込みビューア、画像プレースホルダー、テーブルソーターがあり、web コンポーネントの実用的な用途を示しています。
* **プログレッシブ拡張** JavaScriptの読み込みに失敗した場合に、web コンポーネントで機能を中断することなく既存のHTMLを強化できます。
* **次の手順とリソース** このプレゼンテーションでは、フォームパーティシペーション、宣言型シャドウ DOM、カスタムHTML属性、サーバーサイドレンダリングの調査を提案します。 リソースには、MDN、webcomponents.org、Ben Farrell の著書「Web Components in Action」などがあります。