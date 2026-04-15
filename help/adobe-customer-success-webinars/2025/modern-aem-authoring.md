---
title: 最新のAdobe Experience Manager オーサリング用ユニバーサルエディターの概要
description: AEMのユニバーサルエディター（ユースケース、アーキテクチャ間のサポート、主要な考慮事項）により、コンテンツのオーサリングを簡素化し、配信を促進する方法をご確認ください。
solution: Experience Manager
feature: Authoring
topic: Headless, Integrations, Security
role: Admin, Developer, User
level: Beginner, Intermediate
doc-type: Event
duration: 2891
last-substantial-update: 2025-08-19T00:00:00Z
jira: KT-18763
exl-id: 6212a20d-f58c-481c-a475-89153cb0d040
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 2%

---

# ユニバーサルエディター：最新のAEMオーサリングの戦略的概要

Adobe Experience Managerのユニバーサルエディターが、Edge Delivery Servicesからヘッドレス実装に至るまで、さまざまなアーキテクチャをまたいでコンテンツオーサリングをどのように変革しているかをご確認ください。 このセッションでは、ユニバーサルエディターの実践的なユースケースと、プロジェクトに適しているかどうかを判断するための主要な技術的考慮事項について包括的に解説します。 AEMへのユニバーサルエディターの導入に関する一般的な課題を解決し、十分な情報にもとづいて意思決定する方法を説明します。

## 主な議論ポイント

* ユニバーサルエディターのプライマリ使用例
* AEM Sitesの従来型コンテンツに対応するユニバーサルエディター
* アーキテクチャをまたいだ一般的な技術的考慮事項
* よくある質問

>[!VIDEO](https://video.tv.adobe.com/v/3470850/?learn=on&enablevpops)

## ユニバーサルエディターの機能

* **コア機能** インライン編集、フォームベース編集、モーダルダイアログをサポートしています。
* **統合** ワークフロー、翻訳、マルチサイト管理などのAEM ツールとシームレスに連携します。
* カスタムデータ入力タイプ、タブ、モーダルダイアログ用の&#x200B;**カスタマイズ**&#x200B;拡張ポイント。
* **柔軟性** AEM JCR、GraphQL、Edge Delivery Servicesなど、複数のコンテンツバックエンドと互換性があります。

これらの機能により、ユニバーサルエディターは現代のコンテンツ管理ニーズに対応する汎用性に優れたツールとなります。

## AEM エディターの比較

| 機能 | AEM ページエディター | ユニバーサルエディター |
|--------------------------|-------------------------------|-----------------------------|
| **導入済み** | 2014年（タッチ UI） | 2024年 |
| **コンテンツソース** | AEM JCR | AEM JCR、GraphQL、Edge |
| **UI フレームワーク** | Coral UI | React Spectrum |
| **使用例** | 従来のAEMサイト | ヘッドレス，Edge Delivery |
| **カスタマイズ** | 編集可能テンプレート，スタイルシステム | JSON ロジックスキーマ |
