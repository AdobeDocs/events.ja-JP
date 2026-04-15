---
title: Adobe Admin ConsoleへのMarketoの移行 – （移行前）
description: Adobeでは、ユーザー管理を改善するためにMarketo EngageをAdmin Consoleに移行しています。 自動および自己移行の種類、前提条件、移行後の変更、ベストプラクティス、一般的な落とし穴、サポートについて説明します。 AdobeのExperience League web サイトのセッション録画にアクセスします。
solution: Marketo Engage
feature: Programs, Reporting
topic: Integrations, Security, Migration
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 2280
last-substantial-update: 2025-03-14T00:00:00Z
jira: KT-17483
exl-id: 9c3da83f-9e02-4a2e-9784-10213facf056
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 1%

---

# Adobe Admin ConsoleへのMarketoの移行 – 移行前

Adobeの専門家によるシームレスなMarketoへの移行にご参加ください。

このウェビナーでは、Adobe Customer Experience &amp; Identity Teamを利用して、Marketoへの移行に先手を打つことができます。 Adobe Admin Consoleへのスムーズな移行を実現するための主要なステップ、ベストプラクティス、一般的な課題について説明します。

学習すること，

* 移行前プロセスのステップバイステップ形式のロードマップ
* 移行を簡素化し、落とし穴を回避するためのベストプラクティス
* 移行に関する一般的な懸念に対する専門家の回答

移行を始めたばかりでも、最後のステップに向けて準備しているだけでも、このセッションでは、プロセスを確実に進めるための知識とツールを提供します。 Marketoへの移行をシームレスにするために、このチャンスをお見逃しなく！

>[!VIDEO](https://video.tv.adobe.com/v/3449712/?learn=on&enablevpops)

## 重要な留意点

### 移行の目的と概要

Adobeでは、Marketo EngageをAdmin Consoleに移行し、すべての製品を1つのハブに統合することで、ユーザーの管理とアクセスを改善しています。  Admin Consoleは、Adobe製品、ユーザーの役割、権限、サポートアクセスを管理する中央ハブとして機能します。 MARKETO ENGAGEにアクセスするためのURLは、AdobeのExperience Cloud プラットフォームに変更されます。

### 移行タイプ

* **自動移行** ユーザー数が75人未満で、SSL設定がない組織の場合。 Adobeが移行を処理します。
* **自己移行** SSL設定を持つ組織の場合。 管理者は、移行コンソールを使用して移行プロセスを管理します。

### 移行の前提条件

* システム管理者は同意メールに入力する必要があります。
* SSLは、（Marketo インスタンスではなく）Admin Consoleで設定する必要があります。

### 移行後の変更

* ユーザーは、Adobe IDまたはFederated ID （SSL）を使用してログインします。
* 管理者の役割と権限によって、Admin Consoleのアクセスレベルが決まります。

### ベストプラクティス

* 移行前にユーザーの電子メールを確認し、ロックアウトされたアカウントを解決します。
* 適切な管理者ロールが割り当てられていることを確認します。
* 広告ブロッカーを無効にするか、シークレットモードを使用してログインの問題を回避します。

### 陥りやすい失敗

* 管理者の権限が正しくないと、アクセスが制限される場合があります。
* ブラウザーの拡張機能や広告ブロッカーがアクセスを妨げる場合があります。
* IP ホワイトリスト登録は、Admin Consoleではまだサポートされていませんが、現在開発中です。

### 機能への影響

* 自動化されたメール、API ユーザー、およびmunchkin コードは、移行の影響を受けません。
* 移行は、主にユーザーの認証と管理に影響します。

### サポート

* 問題が発生したユーザーは、Adobe カスタマーケアでサポートケースを開く必要があります。
* 迅速な解決のために、サポートケースにIMS組織IDを含めます。
