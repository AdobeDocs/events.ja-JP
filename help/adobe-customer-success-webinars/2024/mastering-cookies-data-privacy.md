---
title: Privacy-First Analytics - Adobe AnalyticsおよびCustomer Journey Analyticsで Cookie とデータプライバシーをマスターする
description: 今日のデータプライバシーの世界では、データ使用と Cookie の同意の管理が非常に重要です。 このビデオでは、Analytics およびCustomer Journey Analyticsの標準ツールに関するAdobeのベストプラクティスについて説明します。
solution: Analytics, Customer Journey Analytics
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3354
last-substantial-update: 2024-08-28T00:00:00Z
jira: KT-16032
source-git-commit: 12447442bb31bec89d2c82b45cf15a8c99bd34ce
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---


# Privacy-First Analytics:Adobe AnalyticsおよびCustomer Journey Analyticsで Cookie とデータプライバシーをマスターする

今日のデータプライバシーの世界では、データ使用と Cookie の同意の管理が非常に重要です。 このビデオでは、Analytics およびCustomer Journey Analyticsの標準ツールに関するAdobeのベストプラクティスについて説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3432997/?learn=on)

このウェビナーでは、Adobe AnalyticsおよびCustomer Journey Analyticsでの cookie のマスターとデータプライバシーに関するインサイトを提供します。 このセッションでは、データガバナンス、オプトインおよびオプトアウト管理のための同意マネージャーの利用、フォールバックトラッキング、GDPR や CCPA などのプライバシー規制に関連した cookie コンプライアンスなどのトピックに焦点を当てました。 この会議は、参加者に対して、Adobeソリューションにおける適切なデータガバナンスとプライバシー規制への準拠を確保するためのベストプラクティス、ワークフロー、ツールについて説明することを目的としています。

## 重要ポイント

* **同意マネージャーの重要性** 会議では、web サイト上でのデータ収集に対するユーザーの同意を管理および文書化する上で、同意マネージャーが重要な役割を果たしていることを強調しました。&#x200B; 同意マネージャーは、ユーザーにデータ収集慣行を透過的に提示し、オプトインおよびオプトアウトのオプションを提供し、ユーザーの好みに基づいてプロセスを更新することで、データプライバシー法のコンプライアンスを確保します。&#x200B;

* **オプトアウトシナリオのフォールバックトラッキング** このディスカッションでは、ユーザーがデータ収集をオプトアウトするシナリオのソリューションとしてのフォールバックトラッキングの概念を導入しました。&#x200B; フォールバックトラッキングを使用すると、トラッキング Cookie を使用したり個人を識別したりせずに、ドメインページの URL やオプトイン/オプトアウトのステータスなどの最小限のデータ収集が可能になり、オプトアウト状況で一定のレベルのデータ収集コンプライアンスを維持する方法が提供されます。&#x200B;

* **サードパーティ cookie の廃止への対応** 特に、Chromeや Safari などのブラウザーの変化に照らして、サードパーティ cookie の廃止に関する最近のお知らせの影響に対処する方法のガイダンスが提供されました。 Recommendationsでは、DNS サーバー解決に CNAME を使用して、ファーストパーティ cookie の動作を模倣し、プライバシー規制の進化やブラウザーの変更の中で長期的なデータ収集ソリューションのために web SDK に移行することが含まれていました。