---
title: Adobe Experience Manager as a Cloud Serviceでの CDN およびWAFの設定
description: Adobeのエキスパートが共有するカスタマイズ可能な CDN ルール、WAF対策、設定パイプラインを使用して、Adobe Experience Manager as a Cloud Service アプリケーションのパフォーマンスとセキュリティを向上させます。
solution: Experience Manager as a Cloud Service
feature: Security
topic: Performance, Security
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2211
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16574
exl-id: a9f38e79-c707-443d-8b2f-e534ce4dd43d
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Adobe Experience Manager as a Cloud Serviceでの CDN およびWAFの設定

カスタマイズ可能な CDN ルール、WAF対策、設定パイプラインを使用して、Adobe管理 CDN の可能性を最大限に活用します。 Adobeのシニアコンピューターサイエンティスト Marius Petria、Adobeのソフトウェア開発エンジニア Quentin Vecchio、Adobeのソフトウェア開発エンジニア Florian Froese が、Adobe Experience Manager as a Cloud Service アプリケーションのパフォーマンスとセキュリティを向上させる戦略を共有します。

>[!VIDEO](https://video.tv.adobe.com/v/3440603/?learn=on&enablevpops&captions=jpn)

## コミュニティ ディスカッション

Adobe Developers Live コミュニティで会話を続けます [ ディスカッション ](https://adobe.ly/3O0TyYa)。

## キーポイント

* **新しい設定機能の紹介** このプレゼンテーションでは、様々なユースケースに CDN を設定する機能に重点を置いて、クラウドサービスでの CDN の新しい設定機能を紹介します。
* **CDN 設定オプション** 新しいオプションにより、ヘッダーの追加や削除、リクエストパスの書き換え、トラフィックのブロック、クライアントのリダイレクト、別のオリジンへのプロキシ化など、HTTP リクエストおよび応答とのやり取りが可能になります。
* **セキュリティの強化** 新機能には、リクエストパターンに基づいてトラフィックをブロックまたはログに記録するトラフィックフィルタールールや、SQL インジェクションや XSS などの web 攻撃に対する高度な保護のための M WAFの導入が含まれます。
* **宣言的な設定** 設定は、YAML ファイルを使用して行い、Cloud Managerの設定パイプラインを通じてデプロイされるので、すばやく簡単なプロセスになります。
* **リクエストと応答の変換** 新機能を使用すると、リクエスト変換で URL を正規化して不要なクエリパラメーターを削除したり、応答をクライアントに送信する前にヘッダーを設定するための応答変換を使用したりできます。
* **トラフィックフィルターとレート制限** トラフィックフィルターは、特定の IP または国をブロックし、DDoS 攻撃から保護するためにレート制限を実装できます。 レート制限は、クライアント IP、ユーザーエージェント、リクエストパスなど、様々な条件に基づいて設定できます。
* **Monitoring and Analysis Tools** Adobeは、トラフィックと使用状況を分析し、潜在的なセキュリティの脅威を特定および軽減するのに役立つ、Elasticsearch/Kibana や Splunk ダッシュボードなどのツールを提供します。
* **実践的なデモ** このプレゼンテーションには、AEMを使用した CDN 設定のデプロイ方法と、Cloud Managerを使用してエラーを処理し、設定をローカルで検証する方法を示すデモが含まれています。
