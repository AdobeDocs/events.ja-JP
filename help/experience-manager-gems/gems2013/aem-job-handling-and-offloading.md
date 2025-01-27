---
title: AEM 5.6.1 でのジョブ処理とオフロードの概要。
description: 高度なジョブ処理機能の技術的な概要について説明します。 ジョブ処理は、レプリケーションやワークフロー処理などの機能の基盤となるインフラストラクチャです。 改善されたジョブ処理 API と新機能に加えて、検出モジュールについて説明します。
discoiquuid: ee4cd526-7363-4b8e-ad26-c2c937b70327
targetaudience: target-audience advanced
exl-id: bd10465b-6f45-4117-b8a0-1310422f5825
duration: 3750
source-git-commit: 9a297cda953d4414131657f9ac84580aea0eabeb
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# AEM 5.6.1 でのジョブ処理とオフロードの概要。 {#introduction-of-job-handling-and-offloading-in-aem}

ジョブ処理は、レプリケーションやワークフロー処理などの機能の基盤となるインフラストラクチャです。 これは、高度なジョブ処理機能の技術的な概要です。 改善されたジョブ処理 API と新機能に加えて、新しい検出モジュールについて説明します。 オフロードフレームワークは、ジョブの処理と検出の上に構築され、非クラスターインスタンス間でのジョブの配布に焦点を当てます。 オフロードが分散ジョブ処理をどのように拡張するかを詳しく見ていきます。 次に、現在のワークフローのオフロードの実装での使用方法と、独自のプロジェクトでの使用方法を見ていきます。

>[!VIDEO](https://video.tv.adobe.com/v/19580/?quality=9)

*2013 年 7 月 24 日（PT）に配信*

**発表者：**

Adobe、シニアデベロッパー、Carsten Ziegeler

Adobe、リードデベロッパー、Marc Pfaff

発表者のスライド – 第 1 部

[ファイルを入手](assets/jobhandling.pdf)

発表者のスライド – 第 2 部

[ファイルを入手](assets/offloading.pdf)

## 関連リンク {#related-links}

* [Apache Sling イベントとジョブ処理 ](https://sling.apache.org/documentation/bundles/apache-sling-eventing-and-job-handling.html)
* [Discovery API およびその実装 ](https://sling.apache.org/documentation/bundles/discovery-api-and-impl.html)
* [ ジョブのオフロード ](https://docs.adobe.com/docs/en/cq/current/deploying/offloading.html)
