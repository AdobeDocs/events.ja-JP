---
title: コンテンツ配信の最適化 – Edgeのサービスを最大限に活用
description: Edge Delivery Services（EDS）に関するセッションでは、そのアーキテクチャ、ドキュメントベースおよびAEMベースのオーサリングとの統合、迅速なサイト作成、カスタマイズオプション、高性能を維持するためのベストプラクティスについて説明しました。
solution: Experience Manager, Experience Manager as a Cloud Service
feature: Edge Delivery Services
topic: Headless, Integrations, Performance
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3589
last-substantial-update: 2024-12-06T00:00:00Z
jira: KT-16631
exl-id: 2057e491-9ec3-4bfe-b85a-6b74d70822bf
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 1%

---

# コンテンツ配信の最適化：Edgeサービスの能力を引き出す

ここでは、Edge Delivery Services（EDS）の概要とそのアーキテクチャについて説明します。 ユニバーサルエディターを使用して、EDSをドキュメントベースのオーサリングとAEMベースのオーサリングと統合する方法について説明します。 EDSの実際の様子はライブデモで示され、その後、さらなる探索のためのリソースやQ&amp;A セッションが続きます。

>[!VIDEO](https://video.tv.adobe.com/v/3440938/?learn=on&enablevpops)

## 重要な留意点

### EDSの概要

* EDSは、ATMの機能を強化するために設計された、構成可能な一連のサービスです。 &#x200B;
* このソリューションの目的は、迅速な開発サイクルと100%のLighthouse スコアにより、エンゲージメントとコンバージョンを促進する優れた体験を提供することです。 &#x200B;

### オーサリングオプション

* **ドキュメントベースのオーサリング**&#x200B;では、コンテンツ作成にMicrosoft WordやGoogle Docsなどの使い慣れたツールを使用しているため、大規模なトレーニングを行うことなく、すばやくコンテンツを作成できます。 &#x200B;
* **ユニバーサルエディター**&#x200B;は、従来のATM サイトと同様のWYSIWYG インターフェイスを提供し、より詳細で視覚的なコンテンツ制作を可能にします。 &#x200B;

### アーキテクチャ

* EDSは、Amazon Cloud Serviceフレームワーク内で統合されます。 &#x200B;
* サーバーレス実装をサポートしており、従来のオーサーインスタンスやパブリッシャーインスタンスがなくても動作します。 &#x200B;
* キャッシュは、顧客インフラストラクチャレベルとEDS レベルの2つのレベルで実装できます。 &#x200B;

### コンテンツ管理

* ドキュメントベースのオーサリングを利用するには、GitHub アカウント、Google DriveまたはMicrosoft SharePoint、Sidekick プラグイン、コード同期ツールが必要です。 &#x200B;
* IAM オーサリングを使用するEDSには、GitHub アカウント、IAM as a Cloud Service ライセンス、コード同期ツールが必要です。

### 開発と展開

* EDSを使用してサイトを作成するプロセスは迅速であり、多くの場合、1日未満かかります。 &#x200B;
* ローカル開発は、aem up コマンドを使用して実行し、web サイトのローカルバージョンを作成します。
* 変更は、メインブランチに結合する前に、テスト用に機能ブランチにコミットできます。 &#x200B;

### カスタマイズと拡張性

* カスタムコンポーネントは、シンプルなCSSとJavaScriptを使用して作成できます。 &#x200B;
* このアーキテクチャでは、サードパーティ製の統合とカスタムオーサリングソースを利用できます。

### ベストプラクティス

* Vanilla JavaScriptとCSSを使用して、高いLighthouse スコアを維持することをお勧めします。
* Reactのようなライブラリの導入は、パフォーマンスの低下を回避するために慎重に検討し、テストする必要があります。

### サポートとドキュメント

* セットアップとカスタマイズのプロセスをユーザーに説明するための包括的なドキュメントが用意されています。 &#x200B;
* 未解決の問題については、Adobe サポートにお問い合わせください。 &#x200B;
