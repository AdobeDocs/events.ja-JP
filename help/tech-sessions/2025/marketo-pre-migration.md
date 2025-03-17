---
title: MarketoのAdobe Admin Consoleへの移行 – （移行前）
description: Adobeは、ユーザー管理を向上させるために、Marketo EngageをAdmin Consoleに移行しています。 自動および自己移行のタイプ、前提条件、移行後の変更、ベストプラクティス、一般的な落とし穴、サポートについて説明します。 AdobeのExperience League web サイトでセッションの録画にアクセスします。
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 2280
last-substantial-update: 2025-03-14T00:00:00Z
jira: KT-17483
exl-id: 9c3da83f-9e02-4a2e-9784-10213facf056
source-git-commit: 848fa8fee05b315361781059eabb3b19904c78c2
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# MarketoのAdobe Admin Consoleへの移行 – 事前移行

Adobe エキスパートとのシームレスなMarketo移行にご参加ください。

この有益なウェビナーで、Adobeのカスタマーエクスペリエンス &amp; ID チームと共に、Marketoへの移行に先立ってください。 Adobe Admin Consoleへのスムーズな移行を実現するための重要な手順、ベストプラクティス、一般的な課題について説明します。

学習内容

* 事前移行プロセスの段階的なロードマップ
* 移行を簡素化し、落とし穴を回避するためのベストプラクティス
* 移行に関するよくある懸念に対するエキスパートの回答

移行を開始する場合でも、最終的な手順に向けて準備する場合でも、このセッションでは、自信を持ってプロセスを進めるための知識とツールを身に付けることができます。 Marketoの移行をシームレスに進めるこのチャンスをお見逃しなく。

>[!VIDEO](https://video.tv.adobe.com/v/3449712/?learn=on&enablevpops)

## 重要ポイント

### 移行の目的と概要

Adobeでは、Marketo EngageをAdmin Consoleに移行して、すべての製品を 1 つのハブに統合し、ユーザー管理とアクセスを向上させています。  Admin Consoleは、Adobe製品、ユーザーの役割、権限、サポートアクセスを管理する中央ハブとして機能します。 Marketo Engageにアクセスするための URL が、Adobe Experience Cloud Platform に変わります。

### 移行タイプ

* **自動移行** ユーザー数が 75 未満で、SSL を設定していない組織の場合。 Adobeが移行を処理します。
* **セルフ移行**:SSL を設定している組織の場合。 管理者は、移行コンソールを使用して移行プロセスを管理します。

### 移行の前提条件

* システム管理者は、同意メールを完了する必要があります。
* SSL は、（Marketo インスタンスではなく）Admin Consoleで設定する必要があります。

### 移行後の変更

* ユーザーは、Adobe IDまたは Federated ID （SSL）を使用してログインします。
* 管理者の役割と権限によって、Admin Consoleのアクセスレベルが決まります。

### ベストプラクティス

* 移行前に、ユーザーの E メールを確認し、ロックアウトされているアカウントを解決してください。
* 適切な管理者ロールが割り当てられていることを確認します。
* 広告ブロッカーを無効にするか、匿名モードを使用して、ログインの問題を回避します。

### よくある落とし穴

* 管理者権限が正しくないと、アクセスが制限される可能性があります。
* ブラウザー拡張機能と広告ブロッカーが、アクセスを妨げる可能性があります。
* IP の許可リストへの登録は、Admin Consoleではまだサポートされていませんが、現在開発中です。

### 機能への影響

* 自動メール、API ユーザーおよび Munchkin コードは、移行の影響を受けません。
* 移行は、主にユーザー認証と管理に影響を与えます。

### サポート

* 問題が発生した場合は、Adobe カスタマーケアでサポートケースをオープンしてください。
* 迅速な解決を実現するために、サポートケースに IMS 組織 ID を含めます。
