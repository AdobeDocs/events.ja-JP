---
title: Fusion を使用したWorkfront ユーザーアカウントの自動作成
description: Adobe Workfront Fusion と API を使用して、ユーザーアカウントの作成を自動化し、セットアップ時間を 22 分から 60 秒未満に短縮し、効率を向上させる方法について説明します。
solution: Workfront
feature: Workfront Fusion, Workfront API
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
source-git-commit: 91120ff6bfd81c7b3c9218fbbb6dbff9397b37e6
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 1%

---

# Fusion を使用したWorkfront ユーザーアカウントの自動作成

月曜日に急ぎの管理者リクエストが殺到し、新規採用者のオンボーディング、アクセス権限の更新、アカウントの非アクティブ化が始まったとします。 ユーザーアカウントを手動で作成すると、時間がかかり、エラーが発生しやすくなります。 Adobe Admin Consoleで Fusion を使用してアカウントを自動的に作成することにより、ワークフローを合理化し、エラーを減らし、効率を高める方法を説明します。

J.P. Morgan Payments の Kurt Jones 氏が、以下に関するエキスパートのインサイトを紹介します。

* Workfront フォームを使用したユーザーアカウントの取り込みのキャプチャ
* User Management API を使用するAdobe Developer Consoleでのプロジェクトの設定
* Fusion を使用したAdmin Consoleでのアカウント作成の自動化
* Fusion によるWorkfront プロファイルへの追加詳細の更新

>[!VIDEO](https://video.tv.adobe.com/v/3471496/?learn=on&enablevpops)

## 管理者とスケーリングのベストプラクティス

* **Formsをシンプルに** 自動処理を効率化するために必要な情報のみを収集します。
* **プロファイルの標準化** マーケティングの役割にミラーユーザーを使用して、チーム、役割、スケジュールを自動入力します。
* **トレーニングへの投資** 正式な Fusion トレーニングは、採用と自信を促進します。
* **監視と反復** プロセスに時間を割き、フィードバックを収集し、シナリオを調整して継続的な改善を行います。
* **グループ管理者の育成** 学習に熱心なチームメンバーを特定し、指導することで、スケーリングに対する管理者の能力を拡大します。

## 自動化の影響：前後

| **指標** | **手動プロセス** | **自動プロセス** |
|-------------------------------|--------------------|-------------------------|
| **ユーザー作成時間** | 最大 22 分 | **&lt; 60 秒** |
| **関連する手順** | 複数のアプリ | **単一ワークフロー** |
| **エラー率** | より高い | **大幅に低下** |
| **セルフサービス機能** | × | **はい** |
| **管理者関与** | 高 | **最小** |
