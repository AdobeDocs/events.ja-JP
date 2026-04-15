---
title: FusionでWorkfrontユーザーアカウントの作成を自動化
description: Adobe Workfront FusionとAPIを使用してユーザーアカウント作成を自動化し、設定にかかる時間を22分から60秒以下に短縮して、効率性を向上させる方法をご確認ください。
solution: Workfront
feature: Workfront Fusion, Workfront API
topic: Integrations, Development
speaker-name-1: Kurt Jones
speaker-company-1: J.P. Morgan
speaker-title-1: Payments
role: User
level: Intermediate, Experienced
doc-type: Event
duration: 0
last-substantial-update: 2025-08-29T00:00:00Z
jira: KT-18876
exl-id: e8ac62c5-75e5-41d2-94c8-25bcaacd5668
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 1%

---

# FusionでWorkfrontユーザーアカウントの作成を自動化

新規採用者のオンボーディング、アクセス権限の更新、アカウントの非アクティブ化など、緊急の管理者リクエストが氾濫する月曜日の始まりを想像してみてください。 ユーザーアカウントを手動で作成するのは、時間がかかり、ミスが生じやすい場合があります。 Adobe Admin ConsoleのAdobe Workfront Fusionを利用して、ワークフローを合理化し、ミスを減らし、アカウント作成を自動化することで効率を高める方法をご確認ください。

J.P. Morgan PaymentsのKurt Jones氏が、

* Workfront フォームを使用したユーザーアカウント受注の取得
* User Management APIを使用するためのAdobe Developer Consoleでのプロジェクトの設定
* Fusionを使用したAdmin Consoleでのアカウント作成の自動化
* Fusionを使用したWorkfront プロファイルへの追加詳細の更新

>[!VIDEO](https://video.tv.adobe.com/v/3471496/?learn=on&enablevpops)

## 管理者と拡張のベストプラクティス

* **Formsをシンプルにする**&#x200B;重要な情報のみを収集してオートメーションを合理化します。
* **プロファイルの標準化** マーケティング役割にミラーユーザーを使用して、チーム、役割、スケジュールを自動入力します。
* **トレーニングへの投資**&#x200B;正式なFusion トレーニングは、導入と自信を加速させます。
* **監視と反復** プロセスの時間を取り、フィードバックを収集し、継続的な改善のためにシナリオを調整します。
* **グループ管理者の開発**&#x200B;学習を希望するチームメンバーを特定して指導し、管理者のキャパシティを拡大して拡大します。

## 自動化の影響：前後

| **指標** | **手動プロセス** | **自動プロセス** |
|-------------------------------|--------------------|-------------------------|
| **ユーザー作成時間** | ～22分 | **&lt; 60秒** |
| **関与する手順** | 複数のアプリ | **単一のワークフロー** |
| **エラー率** | 上位 | **大幅に下がり** |
| **セルフサービス機能** | × | **○** |
| **管理者の関与** | 高 | **最小** |
