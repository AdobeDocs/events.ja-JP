---
title: Adobe AnalyticsからAdobe Customer Journey Analyticsへの移行に関するベストプラクティス
description: XDM スキーマの設計、データマッピング、データビューの設定など、Adobe AnalyticsからCustomer Journey Analytics（CJA）への移行に必要な手順とベストプラクティスについて説明します。
solution: Analytics, Customer Journey Analytics
feature: Segmentation, Basics, Use Cases, Identity
topic: Migration
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 3654
last-substantial-update: 2025-07-16T00:00:00Z
jira: KT-18535
exl-id: 725291fa-add4-4c93-8bc9-37155936c9d8
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# Adobe AnalyticsからAdobe Customer Journey Analyticsへの移行に関するベストプラクティス

Adobe AnalyticsからCustomer Journey Analytics（CJA）への移行について説明します。 このセッションでは、AdobeのUltimate Success チームのNicolina Picone氏とMaurizio Corò氏がホストを務め、CJAとその機能、移行に関するベストプラクティスについて詳しく説明します。

## 主なトピック

* adobe AnalyticsとCJAの違い
* 強力なID識別子、データ構造の調整、カスタマイズ可能なデータビューの作成の重要性です
* 過去のデータのインポートや、マーケティングチャネルのアトリビューションの管理、CJAの柔軟性を活用したカスタマイズされたレポート作成などの戦略について解説します

>[!VIDEO](https://video.tv.adobe.com/v/3464911/?learn=on&enablevpops)

## 重要なポイント

* **Customer Journey Analytics（CJA）の概要** CJAは、Adobe Analyticsの進化であり、シングルトラックイベントではなく、複数の顧客接点（モバイル、web、CRM、コールセンターなど）をまたいだカスタマージャーニー全体に焦点を当てています。 リアルタイムのデータ処理と操作が可能になります。

* **移行の準備状況** Adobe AnalyticsからCJAへの移行に関する主な手順には、強力なID ID （例：人物ID）の確認、変数とディメンションの調整、データのXDM スキーマへのマッピングが含まれます。 検証ステップで履歴データをインポートすることも可能です。

* **データビューと柔軟性** CJAを使用すると、セッション期間、セグメント化フィルター、アトリビューション設定を調整して、カスタマイズ可能なデータビューを作成できます。 こうした柔軟性により、カスタマイズされたレポートと分析が可能になります。

* **過去データの移行に関するベストプラクティス** CJA データを、許容される範囲内（10%の差など）のAdobe Analytics データと比較して検証します。 短いバックフィルウィンドウ（1か月など）から始め、徐々にスケールアップしていきます。

* **マーケティングチャネルアトリビューション** CJAでは、マーケティングチャネルアトリビューション機能が強化され、「最初の訪問」機能などの制限がなくなり、より動的なセッション設定が可能になります。
