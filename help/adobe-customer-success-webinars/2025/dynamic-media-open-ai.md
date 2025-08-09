---
title: Open API を使用した Dynamic Media のマスター
description: 従来の Dynamic Media と Open API モデルの主な違いを理解し、Open API を使用して Dynamic Media Ultimateを正常に移行および実装する方法を説明します。
solution: Experience Manager as a Cloud Service, Experience Manager Assets
feature-set: Experience Manager Assets
feature: SDK/API
topic: Development, Content Management
role: Admin, Developer, User
level: Beginner, Intermediate
doc-type: Event
duration: 2757
last-substantial-update: 2025-08-08T00:00:00Z
jira: KT-18702
source-git-commit: ef1eacd73c5a4fb9cdfee730d40606ec65bab2a7
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 3%

---


# Open API を使用した Dynamic Media のマスター

このウェビナーは、従来の Dynamic Media に精通し、Open API を使用して [Dynamic Media Ultimate](https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dm-prime-ultimate) を理解し、実装することを検討しているプロフェッショナルを対象としています。  Open API を使用した Dynamic Media Ultimateの高度な動作を探索し、従来の Dynamic Media と比較します。 Dynamic Media を熟知した参加者が Open API モデルに簡単に適応できるようにして、これら 2 つのアプローチの違いを包括的に理解できるようにすることが目標です。

>[!VIDEO](https://video.tv.adobe.com/v/3470620/?learn=on&enablevpops)

## 主な機能の比較

| 機能 | Dynamic Media | Dynamic Media と OpenAPI |
|-----------------------------|------------------------|----------------------------|
| *対象* | オンプレミス、AMS、クラウド | クラウドのみ |
| *修飾子* | 利用可能なリッチセット | 制限はあるが増加中 |
| *アクセス制御* | すべてのユーザーに開く | 役割によって制限 |
| *CDN TTL* | 最大 10 時間 | 最大 10 分 |
| *承認の実施* | 自動公開 | 承認が必要 |
| *SEO に対応* | ○ | ○ |

## 統合シナリオ

これらの統合シナリオは、企業の様々なニーズに対する、OpenAPI を使用した Dynamic Media の柔軟性と拡張性を示しています。

* **AEM Sitesとの統合** Dynamic Media と OpenAPI では、AEM Sitesとのシームレスな統合がサポートされており、アセットを重複せずに配信層から直接取得できます。
* **サードパーティ CMS** API またはマイクロフロントエンドアプリケーションを使用して、Salesforceや Drupal などのプラットフォームと統合できます。
* **API 駆動型アクセス** アセットの最適化されたレンディションを検索、取得、配信するための API を提供します。
* **配信層の最適化** Assetsは Fastly を介して提供され、より迅速で効率的な配信を確保します。