---
title: Adobe Experience Manager as a Cloud ServiceでのDispatcher設定
description: AEM as a Cloud Serviceの拡張性と効率性を最大化するキャッシュ、セキュリティ、パフォーマンスに関するAEM Dispatcherのベストプラクティスをご確認ください。
solution: Experience Manager as a Cloud Service
version: Experience Manager as a Cloud Service
feature: Dispatcher
topic: Security, Performance, Development
role: Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 4200
last-substantial-update: 2025-05-07T00:00:00Z
jira: KT-17903
exl-id: 7c3542c0-74fe-4f9d-8edb-d4bc442deff3
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# 技術セッション：Adobe Experience Manager as a Cloud ServiceでのDispatcher設定

**Adobe Experience Manager （AEM） as a Cloud Service**&#x200B;は、最新のデジタル エクスペリエンス プラットフォームの拡張性、柔軟性、パフォーマンス向上を提供します。 このアーキテクチャの中核となるのは、**AEM Dispatcher**&#x200B;です。これは、キャッシュ、セキュリティ、リクエスト管理を担当する重要なコンポーネントです。 Dispatcherを適切に設定すれば、コンテンツの配信を高速化し、バックエンドシステムを保護して、サイト全体のパフォーマンスを向上できます。

キャッシュ戦略、アクセス制御メカニズム、リクエストフィルタリングなど、Dispatcherの主な設定を紹介します。 また、クラウドで安全でパフォーマンスの高いAEMのデプロイメントを維持するためのベストプラクティスも紹介します。 開発者、アーキテクト、ビジネスの意思決定者のいずれであっても、AEM as a Cloud Serviceの可能性を最大限に引き出すには、Dispatcherの設定をしっかりと理解することが重要です。

>[!VIDEO](https://video.tv.adobe.com/v/3457891/?learn=on&enablevpops)

## 重要な留意点

* **検証用Dispatcher SDK** AEM Dispatcher SDKは、設定の静的な分析のための強力なツールです。 設定をすばやく検証し、不変性をチェックしてエラーを特定できるため、パイプライン全体のデプロイと比較して大幅に時間を節約できます。

* **迅速な開発環境（RDE）** RDEは、静的分析を超えた構成をテストおよびデバッグするためのインタラクティブなランタイム環境を提供します。 これにより、検証とデバッグの速度が向上し、デプロイメントとテストに必要な時間が短縮されます。

* **Mod Proxyを使用した高度なネットワーク** VPNや専用エグレス IPなどの高度なネットワーク設定は、Cloud Managerを使用して設定できます。 Mod プロキシモジュールを使用すると、AEMから外部サービスにトランザクションをオフロードし、パフォーマンスを最適化してJVMの負荷を軽減できます。

* **Dispatcher設定に関するベストプラクティス**&#x200B;主な推奨事項には、相対パス、一意のx-vhost ヘッダー、適切なクライアントヘッダー、キャッシュ制御ヘッダーの活用によるキャッシュの効果的な管理が含まれます。 これらのプラクティスは、パイプラインのエラーを回避し、デバッグ効率を向上させるのに役立ちます。

* **デプロイ用のWeb階層パイプライン** Web階層パイプラインは、分離されたDispatcher設定をデプロイするためのユーティリティです。 キャッシュの無効化などの追加テストが含まれており、コンテンツの更新が本番環境に迅速かつ正確に反映されます。
