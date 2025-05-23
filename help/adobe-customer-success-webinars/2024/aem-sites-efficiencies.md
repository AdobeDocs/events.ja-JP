---
title: AEM Sitesの効率性 – パフォーマンスの最適化、設定、トラブルシューティング
description: AMP サイトの効率性に関するウェビナーでは、パフォーマンスの最適化、Dispatcher の設定、権限管理のベストプラクティス、パフォーマンス上の問題に対処するための戦略について説明しました。
solution: Experience Manager
version: Experience Manager as a Cloud Service
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3452
last-substantial-update: 2024-10-30T00:00:00Z
jira: KT-16353
exl-id: 55f7c1d8-7c2c-4392-894a-2aa9b3cc0e4a
source-git-commit: 5c946ab73e78d4243ca310032a10bb8e82228c3d
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# AEM Sitesの効率性：パフォーマンスの最適化、設定およびトラブルシューティング

このウェビナーでは、Adobe Experience Manager（AEM） Sites のトラブルシューティングの基本事項を説明します。 パフォーマンス上の問題が発生した場合でも、複雑な設定を扱う場合でも、このセッションでは、AEM環境を維持管理し最適化するための実践的なスキルを身に付けることができます。 スライドよりもライブデモの方が優先され、実際の課題に取り組む上での実践的な経験を提供します&#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3435114/?learn=on)

## キーポイント

このウェビナーでは、パフォーマンスの最適化、設定、トラブルシューティングなど、AMP サイトの効率性に焦点を当てました。

### Dispatcher設定

* パフォーマンスの高い web サイトを配信する上での Dispatcher の重要性。
* Dispatcher 設定の主要な側面：仮想ホスト設定、キャッシュ構造を使用したドメインマッピング、通常のレポートとリダイレクト。

### Rights Management

* ベストプラクティス：グループに権限を適用し、拒否ステートメントを避け、過度な使用を避けます。
* Yaml ファイルを通じて権限を管理するための Netcentric ACL ツールの使用。これにより、デプロイメントとトレーサビリティが容易になります。

### パフォーマンスの問題

* キャッシュの完全なフラッシュを避けるために、同期操作でデルタを識別することが重要です。
* 営業時間内に大きなページ操作を行わないようにします。
* 必要な手順へのワークフローを簡素化します。
* オーサーシステム、特に ImageMagick などのツールを使用する場合は、サードパーティのシステムプロセスには注意が必要です。
* 負荷に対応できないサードパーティ製システムへのリクエストを同期させないでください。
* パフォーマンスの低下を避けるために、重いカスタムコンポーネントを管理します。
* セグメントが見つからないという例外を防ぐために、長時間実行されているセッションを監視します。
