---
title: Adobe Experience Manager Edge Delivery Servicesに AI とPersonalizationを導入
description: Cognizant Netcentric のプリンシパルソリューションアーキテクトであるAndreas Haller が示した、基本的なアーキテクチャ、セマンティック検索、高度なユースケースを使用して、Adobe Experience Manager Edge Delivery Servicesに AI とパーソナライゼーションを統合する方法を説明します。
feature: Edge Delivery Services, Search, Generative AI
topic: Artificial Intelligence, Personalization
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1029
last-substantial-update: 2024-11-25T00:00:00Z
jira: KT-16578
source-git-commit: 8770c8172ee90524079efc65aec7e129f1d1d031
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---


# Adobe Experience Manager Edge Delivery Servicesに AI とPersonalizationを導入

パーソナライゼーションと AI をAdobe Experience ManagerのEdge Delivery Servicesに統合する基本的なアーキテクチャについて説明します。 Cognizant Netcentric のプリンシパルソリューションアーキテクトであるAndreas・ハラーが、プロジェクトを強化するためのセマンティック検索と高度なユースケースについて説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3440405/?learn=on&enablevpops)

## コミュニティ ディスカッション

Adobe Developers Live コミュニティで会話を続けます [ ディスカッション ](https://adobe.ly/3Z0PtJF)。

## 重要な留意点

### Personalizationと AI の統合

* Web サービスへの AI とパーソナライゼーションの統合、特に web サイトのコンテンツとユーザーの行動に焦点を当てます。

### 2 段階アプローチ

* **データ収集** 高度な分析やブラウザーデータポイントを使用して、ユーザーデータを収集します。
* **データの解釈** AI 対応バックエンドを使用して、パーソナライズされたコンテンツを処理し表示します。

### デモインサイト

* ユーザーの行動がコンテンツの表示に影響を与える概念実証を実演しました。
* データ収集とコンテンツのマッチングのための意味検索にローカルストレージを利用しました。

### アーキテクチャの概要

* 主なコンポーネントには、ブラウザー、エッジ配信サービス、コンテンツバックエンド、API ゲートウェイなどが含まれます。
* データ取り込みと検索インデックス作成の拡張機能。
* OpenSearch の使用とセマンティック検索へのモデルの埋め込み。
* 完全一致と意味一致を組み合わせたハイブリッド検索アプローチ。

### さらなる拡張の可能性

* チャットボット用の大規模言語モデルの統合。
* 製品レコメンデーションの実装
* パーソナライズされた価格戦略を開発する。
* 基本的な設定から始めて、徐々により複雑なシナリオを作成することに重点を置いています。

### 実用的な実装

* このアプローチを使用すると、ステップバイステップの構築が可能になり、より複雑なユースケースと機能を実現できます。
* AI 機能とパーソナライゼーション機能の実験と段階的な強化を推奨します。
