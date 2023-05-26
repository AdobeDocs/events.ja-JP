---
title: AEM 5.6.1 でのジョブ処理とオフロードの概要。
description: 高度なジョブ処理機能の技術的な概要について説明します。ジョブ処理は、レプリケーションやワークフロー処理などの機能の基盤となるインフラストラクチャです。改善されたジョブ処理 API と新機能に加えて、検出モジュールについて説明します。
uuid: 181e3781-8eca-4a5d-879e-15ae4e1f6649
discoiquuid: ee4cd526-7363-4b8e-ad26-c2c937b70327
targetaudience: target-audience advanced
exl-id: 13888662-d1c5-4fff-b55e-38acede95396
source-git-commit: e401bf0b5ac1e7f06a4576e36887358bed352162
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 96%

---

# AEM 5.6.1 でのジョブ処理とオフロードの概要 {#introduction-of-job-handling-and-offloading-in-aem}

ジョブ処理は、レプリケーションやワークフロー処理などの機能の基盤となるインフラストラクチャです。これは、高度なジョブ処理機能の技術的な概要です。改善されたジョブ処理 API と新機能に加えて、検出モジュールについて説明します。オフロードフレームワークは、ジョブの処理と検出の上に構築され、非クラスターインスタンス間でのジョブの配布に焦点を当てます。オフロードが分散ジョブ処理をどのように拡張するのかを詳しく見ていきます。次に、現在のワークフローのオフロードの実装での使用方法と、独自のプロジェクトでの使用方法を見ていきます。

>[!VIDEO](https://video.tv.adobe.com/v/19580/?quality=9)

*2013年7月24日（PT）に配信*

**発表者：**

アドビ、シニアデベロッパー、Carsten Ziegeler

アドビ、リードデベロッパー、Marc Pfaff

発表者のスライド - 第 1 部

[ファイルを入手](assets/jobhandling.pdf)

発表者のスライド - 第 2 部

[ファイルを入手](assets/offloading.pdf)

## 関連リンク {#related-links}

* [Apache Sling イベントとジョブ処理](https://sling.apache.org/documentation/bundles/apache-sling-eventing-and-job-handling.html)
* [Discovery API およびその実装](https://sling.apache.org/documentation/bundles/discovery-api-and-impl.html)
* [ジョブのオフロード](https://docs.adobe.com/docs/en/cq/current/deploying/offloading.html)
