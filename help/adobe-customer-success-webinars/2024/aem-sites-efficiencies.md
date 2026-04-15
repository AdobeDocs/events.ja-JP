---
title: AEM Sitesの効率性 – パフォーマンスの最適化、設定、トラブルシューティング
description: AMP サイトの効率性に関するウェビナーでは、パフォーマンスの最適化、Dispatcher設定、権限管理のベストプラクティス、パフォーマンスの問題に対処する戦略について説明しました。
solution: Experience Manager
feature: Authoring
topic: Performance
version: Experience Manager as a Cloud Service
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3452
last-substantial-update: 2024-10-30T00:00:00Z
jira: KT-16353
exl-id: 55f7c1d8-7c2c-4392-894a-2aa9b3cc0e4a
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# AEM Sitesの効率性：パフォーマンスの最適化、設定、トラブルシューティング

このウェビナーでは、Adobe Experience Manager（AEM） Sitesのトラブルシューティングの基本について説明します。 パフォーマンスの問題に直面している場合でも、複雑な設定を扱っている場合でも、このセッションでは、AEM環境の保守と最適化を行うための実践的なスキルを提供します。 スライドよりもライブデモを優先し、実際の課題に取り組む実践的な経験を提供します&#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3435114/?learn=on)

## キーポイント

このウェビナーでは、パフォーマンスの最適化、設定、トラブルシューティングなど、AMP サイトの効率性に焦点を当てました。

### Dispatcherの設定

* パフォーマンスの高いweb サイトを提供する上でのDispatcherの重要性。
* Dispatcher設定の主な側面：仮想ホスト設定、キャッシュ構造を使用したドメインマッピング、通常のレポートとリダイレクト。

### Rights Management

* ベストプラクティス：グループに権利を適用し、拒否ステートメントを避け、過剰なエンジニアリングを避けます。
* Netcentric ACL ツールを使用して、Yaml ファイルを通じて権限を管理し、簡単なデプロイメントとトレーサビリティを実現します。

### パフォーマンスの問題

* 完全なキャッシュフラッシュを回避するために、同期操作でデルタを特定することが重要です。
* 営業時間内の大きなページの運用を避ける：
* ワークフローを簡素化し、必要な手順を実行。
* オーサーシステム上のサードパーティシステムプロセス、特にImageMagickなどのツールでは注意が必要です。
* 読み込みを処理できないサードパーティシステムへの同期リクエストを避けます。
* 多量のカスタムコンポーネントを管理して、パフォーマンスの低下を回避できます。
* セグメントが見つからない例外を防ぐために、長時間実行セッションを監視します。
