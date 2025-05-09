---
title: Adobe Experience Manager as a Cloud ServiceでのDispatcher設定
description: AEMのスケーラビリティと効率性を最大限に高めるための、キャッシュ、セキュリティ、パフォーマンスに関するAEM as a Cloud Service Dispatcherのベストプラクティスについて説明します。
solution: Experience Manager as a Cloud Service
version: Experience Manager as a Cloud Service
feature: Dispatcher
role: Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 4200
last-substantial-update: 2025-05-07T00:00:00Z
jira: KT-17903
source-git-commit: cfc7b54ae4360779ca2c41f88fc08089bae99165
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---


# テクニカルセッション：Adobe Experience Manager as a Cloud ServiceでのDispatcher設定

**Adobe Experience Manager（AEM）as a Cloud Service** は、最新のデジタルエクスペリエンスプラットフォームに対して、拡張性、柔軟性、パフォーマンスの向上を提供します。 このアーキテクチャの中心には、キャッシュ、セキュリティ、リクエスト管理を担う重要なコンポーネントである **0}AEM Dispatcher} があります。** Dispatcherを適切に設定すると、コンテンツ配信を高速化し、バックエンドシステムを保護して、サイト全体のパフォーマンスを向上させることができます。

この概要では、キャッシュ方法、アクセス制御メカニズム、リクエストのフィルタリングなど、Dispatcherの主要な設定について説明します。 また、クラウドで安全でパフォーマンスの高いAEMのデプロイメントを維持するためのベストプラクティスについても説明します。 開発者、アーキテクト、ビジネスの意思決定者を問わず、AEM as a Cloud Serviceの可能性を最大限に引き出すには、Dispatcherの設定を十分に理解することが重要です。

>[!VIDEO](https://video.tv.adobe.com/v/3457891/?learn=on&enablevpops)

## 重要な留意点

* **検証用のDispatcher SDK** AEM Dispatcher SDKは、設定の静的分析のための強力なツールです。 設定の迅速な検証、不変性のチェック、エラーの特定が可能で、完全なパイプラインデプロイメントと比較して大幅な時間の節約になります。

* **迅速な開発環境（RDE）** RDE は、静的分析を超えて設定をテストおよびデバッグするためのインタラクティブなランタイム環境を提供します。 検証とデバッグを迅速化し、デプロイメントとテストに要する時間を短縮します。

* **Mod Proxy による高度なネットワーク** VPN や専用エグレス IP などの高度なネットワーク設定は、Cloud Managerを使用してセットアップできます。 mod プロキシモジュールを使用すると、AEMから外部サービスにトランザクションをオフロードでき、パフォーマンスが最適化され、JVM の負荷が軽減されます。

* **Dispatcher設定のベストプラクティス** 主な推奨事項には、相対パス、一意の x-vhost ヘッダー、適切なクライアントヘッダーの使用、キャッシュを効果的に管理するためのキャッシュ制御ヘッダーの活用が含まれます。 これらのプラクティスは、パイプラインのエラーを回避し、デバッグ効率を向上させるのに役立ちます。

* **デプロイメント用の web 階層パイプライン** web 階層パイプラインは、分離された Dispatcher 設定をデプロイするためのユーティリティです。 これには、キャッシュの無効化などの追加テストが含まれ、コンテンツの更新が実稼動環境に迅速かつ正確に反映されるようにします。