---
title: コンテンツ配信の最適化 – Edge サービスのパワーを解き放つ
description: ATM Edge Delivery Services（EDS）は、構成可能なサービス、迅速な開発サイクル、高い lighthouse スコアによりATMの機能を強化し、ドキュメントベースおよびWYSIWYGのオーサリング、サーバーレスのアーキテクチャ、迅速なサイト作成、広範なカスタマイズオプションに対応しています。
solution: Experience Manager, Experience Manager as a Cloud Service
feature: Edge Delivery Services
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3589
last-substantial-update: 2024-12-06T00:00:00Z
jira: KT-16631
source-git-commit: 47ae42d06ed311e60ebce194e0683bb95e8e5b69
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---


# コンテンツ配信の最適化：Edge サービスのパワーを解き放つ

このセッションでは、Edge Delivery Services（EDS）とそのアーキテクチャの概要を説明する。 EDS がユニバーサルエディターを介してドキュメントベースのオーサリングおよびAEMベースのオーサリングとどのように統合するかを詳しく説明します。 ライブデモでは、実際に EDS を見せながら、さらなる調査のためのリソースや Q&amp;A セッションを行います。

>[!VIDEO](https://video.tv.adobe.com/v/3440938/?learn=on&enablevpops)

## 重要ポイント

### EDS の概要

* EDS は、ATMの機能を強化するように設計された、構成可能な一連のサービスです。&#x200B;
* 開発サイクルの高速化と 100% の Lighthouse スコアにより、エンゲージメントとコンバージョンを促進する優れたエクスペリエンスを提供することを目的としています。&#x200B;

### オーサリングオプション

* **ドキュメントベースのオーサリング** Microsoft Word やGoogle ドキュメントなどの使い慣れたツールを使用して、広範なトレーニングを行わずに迅速にコンテンツを作成できます。&#x200B;
* **ユニバーサルエディター** 従来のATM サイトと同様のWYSIWYG インターフェイスを提供し、より詳細で視覚的なコンテンツ作成を可能にします。&#x200B;

### アーキテクチャ

* EDS は、AmazonCloud Serviceフレームワーク内に統合されます。&#x200B;
* サーバーレス実装をサポートしており、従来のオーサーインスタンスまたはパブリッシュインスタンスがなくても動作します。&#x200B;
* お客様のインフラストラクチャ・レベルと EDS レベルの 2 つのレベルのキャッシュを実装できます。&#x200B;

### コンテンツ管理

* ドキュメントベースのオーサリングには、GitHub アカウント、Google Drive またはMicrosoft SharePoint、サイドキックプラグイン、コード同期ツールが必要です。&#x200B;
* IAM オーサリングを使用した EDS には、GitHub アカウント、IAM as a cloud service ライセンス、およびコード同期ツールが必要です。

### 開発とデプロイメント

* EDS を使用してサイトを作成するプロセスは迅速で、多くの場合 1 日未満かかります。&#x200B;
* ローカル開発には、aem up コマンドを使用して web サイトのローカルバージョンを作成します。
* main ブランチにマージする前に、テスト用に機能ブランチに変更をコミットできます。&#x200B;

### カスタマイズと拡張性

* カスタムコンポーネントは、単純な CSS とJavaScriptを使用して作成できます。&#x200B;
* このアーキテクチャを使用すると、サードパーティの統合とカスタムオーサリングソースを利用できます。

### ベストプラクティス

* Vanilla JavaScriptと CSS を使用して、高い Lighthouse スコアを維持することをお勧めします。
* React などのライブラリを導入する場合は、パフォーマンスの低下を避けるために慎重に検討し、テストする必要があります。

### サポートおよびドキュメント

* セットアップとカスタマイズのプロセスを順を追って説明する包括的なドキュメントが利用できます。&#x200B;
* 未解決の問題がある場合は、Adobeサポートにお問い合わせください。&#x200B;