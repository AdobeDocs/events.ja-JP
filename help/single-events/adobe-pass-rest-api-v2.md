---
title: Adobe Pass – 新しいREST API v2
description: このセッションでは、Adobeの新しいREST API v2の概要と、移行プロセスを通じてユーザーを導くことに焦点を当てます。
role: Developer
solution: Pass
feature: APIs
topic: Integrations, Migration
level: Beginner, Intermediate, Experienced
doc-type: Technical Video
duration: 3230
last-substantial-update: 2025-04-07T00:00:00Z
jira: KT-17685
hidefromtoc: true
exl-id: 745411bb-48d7-4410-a236-d02c2927ac1b
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Adobe Pass – 新しいREST API v2

このセッションでは、Adobeの新しいREST API v2の概要と、移行プロセスを通じてユーザーを導くことに焦点を当てます。

>[!VIDEO](https://video.tv.adobe.com/v/3457461/?learn=on&enablevpops)

## 新機能ハイライト

* **概要と利点**

   * REST API v2は、モダンで柔軟性の高い、スケーラブルな認証向けに設計されており、需要の高いイベントやマルチデバイスのシナリオに対応します。
   * 主な改善には、暗号化の強化、セッションの一貫性、クロスデバイス SSO、デバッグを高速化するための拡張エラー情報が含まれます。

* **移行手順**

   * ユーザーは、REST API v2 スコープを使用して新しい登録済みアプリケーションを作成する必要があります。
   * デバイス識別やMVPD マッピングなどの既存の設定を再利用できます。
   * 移行には、登録、設定、認証、事前認証、承認などのフェーズがあります。

* **機能強化**

   * 統合されたRESTful APIがAccess Neighbor SDKに取って代わり、プラットフォーム間の実装が簡素化されます。
   * 同じセッション内の複数の認証プロファイルと、シームレスなクロスデバイス移行をサポートします。
   * コンテンツへのアクセスには、事前承認フローと承認フローが引き続き必須です。

* **タイムライン**

   * REST API v1は、2025年12月までに更新の受信を停止し、2026年末までに完全に廃止されます。
   * ユーザーは、この期限の前に移行を完了することをお勧めします。

* **リソースとサポート**

   * ドキュメント、クックブック、FAQは、Adobe Experience Leagueで入手できます。
   * Adobeでは、サンドボックス環境、Zendesk チケット、移行ミーティングをサポート対象として提供しています。

* **Q&amp;Aのハイライト**

   * REST API v2はv1との下位互換性がないため、再認証が必要です。
   * 事前認証はUI目的ですが、メディアトークンには認証が必要です。
   * SSOは新しいAdobe サービストークンでサポートされています。
