---
title: Adobe Pass – 新しい REST API v2
description: このセッションでは、Adobeの新しい REST API v2 の紹介と、移行プロセスのガイドを中心に説明します。
role: Developer
level: Beginner, Intermediate, Experienced
doc-type: Technical Video
duration: 3230
last-substantial-update: 2025-04-07T00:00:00Z
jira: KT-17685
hidefromtoc: true
source-git-commit: 1082d67d49901e151115255b585799a5f57bda4a
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---


# Adobe Pass – 新しい REST API v2

このセッションでは、Adobeの新しい REST API v2 の紹介と、移行プロセスのガイドを中心に説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3457461/?learn=on&enablevpops)

## 主なハイライト

* **概要とメリット**

   * REST API v2 は、最新の柔軟でスケーラブルな認証用に設計されており、需要の高いイベントやマルチデバイスシナリオに対応します。
   * 主な改善点には、暗号化の強化、セッションの一貫性、クロスデバイス SSO、迅速なデバッグを実現する拡張されたエラー情報などがあります。

* **移行手順**

   * ユーザーは、REST API v2 スコープを使用して、新しい登録アプリケーションを作成する必要があります。
   * デバイス ID やMVPD マッピングなどの既存の設定は再利用できます。
   * 移行には、登録、設定、認証、事前認証、認証などのフェーズが含まれます。

* **機能の強化**

   * 統合 RESTful API は、Access Neighbor SDK に代わるもので、プラットフォーム間の実装を簡素化します。
   * 同じセッション内での複数の認証プロファイルのサポートと、シームレスなクロスデバイス移行。
   * コンテンツへのアクセスには、事前認証フローと認証フローが引き続き必須です。

* **タイムライン**

   * REST API v1 は、2025 年 12 月までに更新の受信を停止し、2026 年末までに完全に廃止されます。
   * ユーザーは、これらの期限よりも十分前に移行を完了することをお勧めします。

* **リソースとサポート**

   * ドキュメント、クックブックおよび FAQ は、Adobe Experience League で入手できます。
   * Adobeは、サポートを目的として、サンドボックス環境、Zendesk チケット、移行ミーティングを提供しています。

* **Q&amp;A のハイライト**

   * REST API v2 は v1 と下位互換性がないので、再認証が必要です。
   * 事前認証は UI 用ですが、メディアトークンには認証が必要です。
   * SSO は新しいAdobe サービストークンを介してサポートされています。

