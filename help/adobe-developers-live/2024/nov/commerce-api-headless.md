---
title: ヘッドレス実装向けCommerce API の調整
description: Adobeのソフトウェアエンジニアである Revanth Kumar が API メッシュを使用して、複数のデータソースを統合および管理し、セキュリティ、パフォーマンス、開発の簡略化などのメリットを得て、高パフォーマンスのヘッドレスコマースエクスペリエンスを実現する方法を説明します。
solution: Commerce
feature: APIs, Headless
topic: Commerce, Development, Headless
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 3304
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16575
exl-id: d12d16c9-3696-48ac-9768-e87aad5191be
source-git-commit: 07d4174b0d89ba2c417866e76ae72f015b91b03a
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# ヘッドレス実装向けCommerce API の調整

Adobeのソフトウェアエンジニア、Revanth Kumar が API メッシュを使用して、複数のソースからの API をつなぎ合わせ、ローコード環境で拡張、変換、配布する方法を説明します。 パフォーマンスの高いヘッドレスコマースエクスペリエンスを簡単に提供します。

>[!VIDEO](https://video.tv.adobe.com/v/3440402/?learn=on&enablevpops)

## コミュニティ ディスカッション

Adobe Developers Live コミュニティで会話を続けます [ ディスカッション ](https://adobe.ly/40IDxO9)。

## 重要な留意点

* **API メッシュの概要**
   * API メッシュは、複数のデータソースを 1 つのGraphQL エンドポイントに組み合わせ、フロントエンド開発者向けの開発プロセスを簡素化するツールです。
   * 広範なGraphQL プロキシとして機能し、セキュリティの向上、スロットリング、DDoS 対策などのメリットを提供するほか、コードの少ない、またはコードなしでビジネスロジックを追加できます。
* **API メッシュの利点**
   * 複数のデータソースを 1 つのエンドポイントに組み合わせることで、それらのデータソースの処理を簡略化します。
   * アプリケーションのパフォーマンスとセキュリティを強化します。
   * バックエンドリソースの負荷を軽減し、安定性と堅牢性を向上させます。
   * デプロイメントプロセスを迅速化し、変更を容易かつ迅速に行います。
* **API メッシュの機能**
   * REST エンドポイント、GraphQL、JSON スキーマなど、様々なデータソースをサポートしています。
   * フィルタースキーマおよびプレフィックススキーマを使用したデータ変換および競合管理が可能です。
   * CORS ヘッダーの設定、キャッシュ、カスタムロジックを追加するためのフック、シークレット管理などの高度な機能を提供します。
* **実践的証明**
   * このセッションには、メッシュの作成、ソースの追加、デプロイなど、API メッシュのセットアップおよび使用方法を示すライブ デモが含まれています。
   * 共同作業による開発に GitHub コードスペースを使用し、メッシュのデプロイメントに CI/CD ワークフローを自動化する方法を実演しました。
   * デバッグとトラブルシューティング**API メッシュのデバッグに VS Code を使用する方法（ブレークポイントの設定や応答の検査など）について説明しました。
   * パフォーマンスを向上させるために、キャッシュや Fastly などの CDN の使用が重要であることを強調しました。
* **地域貢献の推進**
   * ユーザーに、新しい例や機能強化を含んだプルリクエストを作成することで、API メッシュの例リポジトリに投稿することを推奨しました。
