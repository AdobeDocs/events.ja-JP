---
title: Web コンポーネントを使用した独自のHTMLのロール
description: Adobe Adobeの開発者エバンジェリストであるRaymond Camden氏は、カスタムエレメント、Shadow DOM、HTMLテンプレートなど、web コンポーネントの基本を学ぶことができます。また、PDFの埋め込みや並べ替え可能なテーブルの構築などの実用的な例も示され、アプリケーションの強化に役立ちます。
feature: Edge Delivery Services, Release Information
topic: Development
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2580
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16579
exl-id: 57651e92-35d0-4f5a-b4bb-157f62347527
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Web コンポーネントを使用した独自のHTMLのロール

Adobeのシニア開発者エバンジェリストであるRaymond Camden氏が、カスタムエレメント、Shadow DOM、HTML テンプレートなどのweb コンポーネントの基本を学びます。 PDFの埋め込みや並べ替え可能なテーブルの構築など、実例を紹介し、再利用可能な最新のソリューションでアプリケーションを強化します。

>[!VIDEO](https://video.tv.adobe.com/v/3440406/?learn=on&enablevpops)

## コミュニティ議論

Adobe Developers Live コミュニティ [&#x200B; ディスカッション &#x200B;](https://adobe.ly/48PRE63)で引き続きディスカッションを行います。

## 重要な留意点

* **Web コンポーネントの概要** Web コンポーネントを使用すると、開発者は、JavaScriptを使用して定義された、独自の外観とインタラクティブ性を持つカスタム HTML要素を作成できます。
* **コアテクノロジー** Web コンポーネントは、3つのコアテクノロジー**カスタム要素、シャドウ DOM、およびHTML テンプレートを使用して構築されます。
* **カスタム要素** カスタム要素を使用すると、新しいHTML タグを作成できます。 ケバブケースを使用し、ダッシュを含める必要があります。 JavaScript クラスは、ビヘイビアーを定義するために使用されます。
* **シャドウ DOM** シャドウ DOMは、コンポーネントのDOM ツリーのカプセル化を提供し、CSSの漏洩を防ぎ、より制御されたスタイル設定を可能にします。
* **HTML テンプレート** HTML テンプレートを使用すると、HTMLとCSSを複製してDOMに追加できます。 ただし、プレゼンターは、より良い配布と柔軟性のために、テンプレートよりもスロットを使用することを好みます。
* **属性とイベント** カスタム要素には、属性とイベントハンドラー（connectedCallbackやdisconnectedCallbackなど）を設定して、DOMに追加または削除されたときの動作を管理できます。
* **スロット** スロットを使用すると、web コンポーネントにコンテンツを挿入できます。これにより、デフォルトのスロットと名前付きのスロットの両方をサポートし、より柔軟なコンテンツ管理が可能になります。
* **実際の例**&#x200B;例には、PDF埋め込みビューア、画像プレースホルダー、テーブルソーターがあり、web コンポーネントの実用的な用途を示しています。
* **プログレッシブ強化** Web コンポーネントは、JavaScriptの読み込みに失敗した場合、機能を損なうことなく、既存のHTMLを強化できます。
* **次の手順とリソース** フォームへの参加、宣言型シャドウ DOM、カスタム HTML属性、サーバーサイドのレンダリングについて説明します。 リソースには、MDN、webcomponents.org、およびBen Farrellによる著書“ Web Components in Action ”があります。
