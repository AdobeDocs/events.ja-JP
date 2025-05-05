---
title: Assets移行ブループリント
description: 関係者の分析、リソース計画、データ変換、CSV ファイルを使用したデータ処理などのベストプラクティスなど、Achim Koch のインサイトを活用して従来の DAM をAdobe Experience Manager Assetsに移行する方法について説明します。
feature: Migration
topic: Migration
solution: Experience Manager, Experience Manager Assets
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1690
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16576
exl-id: f588055b-05c7-44df-be67-799a0e3ee1ed
source-git-commit: 946d7cd484e8c5d4358d4099b3518705cab8d4a3
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Assets移行ブループリント

Adobeのプリンシパルテクニカルアーキテクト、Achim Koch が、従来の DAM をAdobe Experience Manager Assetsに移行する方法を説明します。 関係者の分析、リソース計画、データ変換、データ処理に CSV ファイルを使用するなどのベストプラクティスに関するインサイトを得ます。 独自のAdobe Experience Manager移行プロジェクトのロードマップを作成します。

>[!VIDEO](https://video.tv.adobe.com/v/3440440/?learn=on&enablevpops&captions=jpn)

## コミュニティ ディスカッション

Adobe Developers Live コミュニティで会話を続けます [ ディスカッション ](https://adobe.ly/4hKHpnF)。

## 重要ポイント

* **移行専用の標準ツールはありません** 製品やカスタムソリューションの多様性のため、様々なレガシーシステムからAdobe Experience Manager（AEM）に移行できるツールは 1 つではありません。

* **移行の 5 つのステージ**

   * プロジェクト計画
   * 実装計画
   * AEMの実装
   * 移行スクリプトの実装
   * 移行の実行

* **関係者の関与** スポンサー、ビジネスユーザー、IT システム管理者、レガシーシステムのサポートなどの関係者を特定し、関与させることが重要です。

* **リソースとタイムラインの計画** リソースが使用可能であることを確認し、休日、ピーク時のビジネスタイム、およびオフリミットの時間枠内で計画します。

* **技術計画** これには、要件分析、データ変換、インフラストラクチャ計画が含まれます。

* **反復プロセス** 移行では、スクリプトの実行、分析、フィードバックおよび適応を複数回繰り返す必要があります。

* **CSV ファイルの使用** CSV ファイルは、移行プロセス中に使用しやすく読みやすいので、推奨されます。

* **スクリプト言語** CSV、AWS、HTTP をサポートしており、JavaScriptを学ぶ良い機会である Node.js をお勧めします。

* **品質と再現性** 高品質のデータ移行を確保し、元のデータと CSV ファイルを参照用に保持して、プロセスを繰り返し可能にします。

* **コンテンツの凍結** 移行中にコンテンツの凍結を宣言して、スナップショットの取得後に新しいデータが追加されないようにします。

* **ツールとヒント** Rainbow CSV 拡張子を持つ VS Code などのツールを使用し、UTF-8 テキストファイルのバイト順序マーカー（BOM）を検討します。

* **ビジネスの承認** 移行後にテストを実施し、正式なビジネス承認を得るための時間を確保して、コンテンツの凍結を解除します。
