---
title: プライバシー重視の分析 – Adobe AnalyticsとCustomer Journey AnalyticsにおけるCookieとデータプライバシーの管理
description: 今日のデータプライバシーの世界では、データ消費とCookie同意の管理が最も重要です。 このビデオでは、AnalyticsとCustomer Journey Analyticsのすぐに使えるツールに関するAdobeのベストプラクティスについて説明します。
solution: Analytics, Customer Journey Analytics
feature: Data Governance, Data Configuration and Collection, Basics, Use Cases
topic: Security, Administration
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3354
last-substantial-update: 2024-08-28T00:00:00Z
jira: KT-16032
exl-id: d2ab94b7-7324-41cf-a2ef-551aa629a3d2
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# プライバシーを重視した分析：Adobe AnalyticsとCustomer Journey AnalyticsでCookieとデータプライバシーを管理

今日のデータプライバシーの世界では、データ消費とCookie同意の管理が最も重要です。 このビデオでは、AnalyticsとCustomer Journey Analyticsのすぐに使えるツールに関するAdobeのベストプラクティスについて説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3432997/?learn=on)

このウェビナーでは、Adobe AnalyticsとCustomer Journey AnalyticsにおけるCookieとデータプライバシーの管理に関するインサイトを提供します。 このセッションでは、データガバナンス、オプトインとオプトアウトの管理における同意管理の活用、フォールバック追跡、GDPRやCCPAなどのプライバシー規制に関するCookie コンプライアンスなどのトピックに焦点を当てました。 このミーティングでは、Adobeソリューション内での適切なデータガバナンスとプライバシー規制への準拠を確保するためのベストプラクティス、ワークフロー、ツールについて、参加者に情報を提供することを目的としています。

## 重要な留意点

* **同意管理の重要性**&#x200B;この会議では、web サイトでのデータ収集に対するユーザーの同意の管理と文書化における同意管理の重要な役割が強調されました。 &#x200B;同意マネージャーは、データ収集の方法をユーザーに透明性を持って提示し、オプトインおよびオプトアウトオプションを提供し、ユーザーの好みに基づいてプロセスを更新することで、データプライバシー法の遵守を徹底します。 &#x200B;

* **オプトアウトシナリオのフォールバックトラッキング**&#x200B;このディスカッションでは、ユーザーがデータ収集をオプトアウトするシナリオの解決策として、フォールバックトラッキングの概念を紹介しました。 フォールバックトラッキング&#x200B;使用すると、Cookieを使用したり個人を特定したりすることなく、ドメインページのURLやオプトイン/オプトアウトステータスなどの最小限のデータ収集が可能になり、オプトアウト状況において一定のデータ収集コンプライアンスを維持できます。 &#x200B;

* **サードパーティ Cookieの廃止に対処する**&#x200B;特にChromeやSafariなどのブラウザーの変化を考慮して、サードパーティ Cookieの廃止に関する最近の発表の影響に対処する際のガイダンスが提供されました。 CNAMEをDNS サーバー解決に利用してファーストパーティ Cookieの動作を模倣し、進化するプライバシー規制やブラウザーの変化の中で長期的なデータ収集ソリューションをweb SDKに移行する方法に関する推奨事項が含まれています。
