---
title: 技術セッション - Campaign コントロールパネルでのAdobe Campaign サブドメインとSSL管理
description: Adobe Campaignのドメイン内でサブドメインをデリゲートおよび設定する方法、SSLCampaign コントロールパネルを設定する方法、および安全なメール配信を確保するための設定を監視する方法について説明します。
solution: Campaign
feature: Subdomains and Certificates
topic: Security, Certification, Development
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3409
last-substantial-update: 2025-09-05T00:00:00Z
jira: KT-18866
exl-id: 2ccb1f70-17fe-444e-b819-2e6daeb8f79d
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# 技術セッション：Campaign コントロールパネルでのAdobe Campaign サブドメインとSSL管理

このセッションでは、サブドメインを保護するためのSSL証明書のインストールなど、Adobe Campaign内でのサブドメインのデリゲーションと設定の概念について説明します。

サブドメインとは何か、その目的、およびAdobeがサブドメインを効果的に使用できるようにするデリゲーション方法について説明します。 このセッションでは、SSL証明書を通じてサブドメインを保護する原則と、安全な環境を維持するためのベストプラクティスについても説明します。

セルフサービスCampaign コントロールパネルを使用してサブドメインを設定する際のステップバイステップのガイダンスを提供し、潜在的な障害とその対処方法を強調します。 参加者は、サブドメインのスムーズなセットアップと安全な管理を確保するための実用的な知識を得ることができます。

管理者、開発者、プラットフォームオーナーのいずれであっても、このセッションでは、Adobe Campaignで自信を持ってサブドメインを設定し、保護するためのスキルを習得できます。

>[!VIDEO](https://video.tv.adobe.com/v/3471391/?learn=on&enablevpops)

## Adobe Campaignでのサブドメイン管理の習得

Adobe Campaignの電子メールコミュニケーションには、サブドメインのデリゲーション、設定、セキュリティなど、必要な機能が揃っています。

* **サブドメインのデリゲーション**&#x200B;完全デリゲーションまたはCNAME デリゲーションのいずれかを選択して、AdobeがDNSとメールの配信品質を管理する方法を制御します。
* **DNSとSSLの設定** MX、SPF、DKIM、DMARC、およびSSL証明書を適切に設定することは、安全で評判の良いメール送信に不可欠です。
* **Campaign コントロールパネル** Adobeのセルフサービス ツールを使用して、サブドメインの設定を効率化し、レコードを監視し、SSL証明書を管理します。
* **一般的な落とし穴**&#x200B;監査タイムライン、レコード要件、トラブルシューティング手順を理解することで、遅延やエラーを回避できます。

これらのプロセスを習得することで、施策の安全性と到達性を高め、ブランドの評判を維持することができます。

## 委任メソッド** FullとCNAMEの比較

* **完全委任** Adobeは、サブドメインのすべてのDNS レコードを管理し、最適な配信品質とセキュリティを確保します。 ほとんどのユーザーに推奨されます。
* **CNAME Delegation**&#x200B;お客様とAdobeは、DNSの責任を共有しています。 お客様は、Adobeで管理されているリソースを指すCNAME レコードを作成します。
* ** 主な違い：
* **Full** Adobeは完全な権限を持っています。お客様によるメンテナンスは少なくなります。
* **CNAME**&#x200B;共有責任。お客様の手作業の手順が増えています。
* **ヒント** メインドメインに対する制御を失わないように、ルートドメイン（サブドメインのみ）を絶対にデリゲートしないでください。
