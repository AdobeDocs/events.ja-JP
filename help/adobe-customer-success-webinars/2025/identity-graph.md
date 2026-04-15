---
title: ID グラフのユースケースとトラブルシューティング
description: Adobe Experience Platform Identity Serviceが、マーケティングの課題を解決するために、セグメンテーション、アクティベーション、プロファイル統合をどのように活用するのかをご確認ください。
feature: Identities, Profiles, Segments
topic: Personalization, Security, Administration
solution: Experience Platform
role: Admin, Developer, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3232
last-substantial-update: 2025-09-24T00:00:00Z
jira: KT-19286
exl-id: ffe6ced7-998c-4e40-a91f-e34e5174dc2c
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# ID グラフのユースケースとトラブルシューティング

このウェビナーでは、Adobe Experience Platform Identity Serviceがどのようにデジタルマーケティングマネージャーにセグメンテーションとアクティベーションのシナリオを考案するための知識を提供するのかを解説します。 マルチデバイスやその他のユースケースの仕組みを正確に把握することで、現実的な現実世界のソリューションが可能になります。

* プロファイル結合の性質/制限をより深く理解する。 これにより、より多くの関係者がセグメンテーションとアクティベーションのシナリオを考案できるようになります。
* 考えられるプロファイルの折りたたみ問題の最初の行の識別。
* ID サービスとリアルタイムの顧客プロファイルの違い。

>[!VIDEO](https://video.tv.adobe.com/v/3475214/?learn=on&enablevpops)

## Identity Graph Essentials

ID グラフは、Adobe Experience Platformの顧客データ統合の基盤です。 電子メール、CRM ID、ロイヤルティカード、Cookie、デバイス IDなど、複数のIDをチャネルやデバイスをまたいでリンクします。

* **ID サービス** データの取り込みとイベントから識別子のペアを接続して、グラフを作成します。
* **プロファイルサービス** グラフを使用してプロファイルフラグメントを統合し、属性、行動、IDを組み合わせて、統合された顧客像を作成します。
* **結合ポリシー** データの競合を最新（タイムスタンプ）またはデータセット権限で解決する方法を決定します。
* **ビジネスへの影響**&#x200B;適切な設定により、正確なレポート、マーケティングの適格性、GDPRなどの規制への準拠が保証されます。

## 顧客データ接続の実現

Adobe Experience PlatformのID グラフルールを活用して顧客データを統合し、より詳細なインサイトとビジネス成果を実現する方法をご確認ください。

* **ID グラフ** デバイスとチャネル間の顧客インタラクションをリンクして、包括的なプロファイルを作成します。
* **名前空間の優先度** ビジネス主導のルールでは、どの識別子（電子メール、CRM ID、ロイヤルティカード）がプロファイルを固定し、競合を解決するかを決定します。
* **結合ポリシー** タイムスタンプまたはデータセットの優先順位を使用して、異なるソースからのデータを組み合わせる方法を制御します。
* **グラフの折りたたみと修正**&#x200B;共有デバイス、未検証データ、または実装エラーは、プロファイルを断片化する可能性があります。シミュレーションツールと修復ジョブは、精度の回復に役立ちます。

これらの概念を理解することで、データ価値を最大化し、コンプライアンスを確保し、パーソナライズされた体験を提供できるようになります。
