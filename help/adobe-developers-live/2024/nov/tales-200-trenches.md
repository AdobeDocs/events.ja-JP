---
title: 200 の堀から伝わる物語
description: パフォーマンスの優先順位付け、Google PageSpeed Insights の使用、LCP や TBT などの主要指標の最適化、リソースの効率的な管理、開発と画像の最適化に関するベストプラクティスに従うことで、web プロジェクトが確実に成功するようにします。
solution: Experience Manager, Experience Manager Sites
feature: Edge Delivery Services
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1321
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16541
source-git-commit: 07d4174b0d89ba2c417866e76ae72f015b91b03a
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---


# 200 の堀から伝わる物語

200 を超えるEdge Delivery Servicesプロジェクトが完了したので、Adobeのシニアエンジニアである Kiran Murugulla と、Adobe Experience Manager Cloud のアーキテクトである Varun Mitra が、主な教訓を共有します。 優れた Core Web Vitals を使用して、高速でパフォーマンスの高いエクスペリエンスを実現する秘訣を見つけます。


>[!VIDEO](https://video.tv.adobe.com/v/3439424/?learn=on&enablevpops)

## コミュニティ ディスカッション

Adobe Developers Live コミュニティで会話を続けます [ ディスカッション ](https://adobe.ly/4fwWvvi)。

## 重要ポイント

* **パフォーマンスが重要** web プロジェクトの成功の重要な要因として、パフォーマンス、特に web ページの速度が強調されます。 第一の目標は、パフォーマンススコアを 100 に保つことです。
* **開発の方法**
   * 開発中の継続的なテストには、Google PageSpeed Insights を使用します。
   * 高いパフォーマンスを維持するために、既に 100 のスコアを付けたボイラープレートコードを使用してプロジェクトを開始します。
   * 結合する前に、プルリクエスト（PR）がパフォーマンス標準を満たしていることを確認します。
* **主要指標** パフォーマンススコアに大きな影響を与える最大コンテンツペイント（LCP）と合計ブロッキング時間（TBT）の最適化に焦点を当てています。
* **リソースの管理**
   * フォントやサードパーティスクリプトなど、必要なリソースをプロジェクトソース内に含めます。
   * 読み込み時間を短縮するには、フォントのフォールバックを使用します。
   * 初期読み込みパフォーマンスを向上させるために、不要なスクリプトの読み込みを遅延させます。
* **画像の最適化** 折りたたまれた画像より上位の画像の読み込みを優先し、重要な画像には優先度の高い取得の設定を使用します。
* **導入事例**
   * ***CNN.com*** パフォーマンスを向上させるために、クエリインデックスを最適化し、Google広告の読み込みを遅延させました。
   * ***Herbert ホーム*** ユーザーがスクロールしたときにデータを読み込み、パフォーマンスとユーザーエクスペリエンスを向上させるために積集合オブザーバー API を使用しました。
* **ベストプラクティス**
   * まずボイラープレートコードから始めて、適切に構成されたマークアップを使用します。
   * 高度な CSS セレクターを利用し、JavaScript操作を最小限に抑えます。
   * モバイルファーストの開発に重点を置きます。
   * 作成者にとって直観的なコンテンツ構造を確保する
* **ツール** サイトのパフォーマンススコアの経時的な追跡に、Google シートや DSA などのツールを使用します。

