---
title: Adobe AnalyticsからAdobe Customer Journey Analyticsへの移行に関するベストプラクティス
description: XDM スキーマ設計、データマッピング、データビュー設定など、Adobe AnalyticsからCustomer Journey Analytics（CJA）への移行に不可欠な手順とベストプラクティスについて説明します。
solution: Analytics, Customer Journey Analytics
topic: Migration
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 3654
last-substantial-update: 2025-07-16T00:00:00Z
jira: KT-18535
source-git-commit: 90eb4a9d2cf445c58fde776092fb047f820fa207
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# Adobe AnalyticsからAdobe Customer Journey Analyticsへの移行に関するベストプラクティス

Adobe AnalyticsからCustomer Journey Analytics（CJA）への移行について説明します。 このセッションは、AdobeのUltimate Success チームの Nicolina Picone と Maurizio Corò がホストし、CJAの概要、機能、移行に関するベストプラクティスを説明します。

## 話し合った主要なトピック

* analytics とCJAの違い
* 強力な ID 識別子、データ構造の調整、カスタマイズ可能なデータビューの作成の重要性
* 履歴データの読み込み、マーケティングチャネルアトリビューションの管理、カスタマイズされたレポートを柔軟にCJAで活用するための戦略について説明します

>[!VIDEO](https://video.tv.adobe.com/v/3464911/?learn=on&enablevpops)

## 重要な高速道路

* **Customer Journey Analytics（CJA）の概要** CJAは、Adobe Analyticsの進化形であり、1 つの追跡イベントではなく、複数のタッチポイント（モバイル、web、CRM、コールセンターなど）にわたる完全なカスタマージャーニーに焦点を当てています。 リアルタイムのデータ処理と操作が可能です。

* **移行への対応** Adobe AnalyticsからCJAへの移行の主な手順には、強力な ID 識別子（例：人物 ID）の確保、変数とディメンションの調整、XDM スキーマへのデータのマッピングが含まれます。 履歴データは、検証手順と共にインポートできます。

* **データビューと柔軟性** CJAを使用すると、セッション時間、セグメント化フィルター、アトリビューション設定を調整して、カスタマイズ可能なデータビューを作成できます。 この柔軟性により、カスタマイズされたレポート作成および分析が可能になります。

* **履歴データ移行のベストプラクティス** 許容範囲内（例：10% の違い）でCJA データをAdobe Analytics データと比較して、検証します。 最初は短いバックフィルウィンドウ（例：1 か月）から開始して、徐々にスケールアップします。

* **マーケティングチャネルアトリビューション** CJAは、マーケティングチャネルアトリビューションの機能強化を提供し、「訪問の最初のページ」機能などの制限を排除し、より動的なセッション設定を可能にします。
