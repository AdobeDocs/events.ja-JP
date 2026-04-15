---
title: 200 Trenchesの記事
description: GoogleのPageSpeed Insightsを活用してパフォーマンスの優先順位付けを行い、LCPやTBTなどの主要指標を最適化し、リソースを効率的に管理し、開発と画像の最適化に関するベストプラクティスに従って、web プロジェクトを成功に導きましょう。
solution: Experience Manager, Experience Manager Sites
feature: Edge Delivery Services
topic: Integrations, Performance, Development
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1321
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16541
exl-id: 1104048d-4074-49aa-a0bc-0065fa2df505
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 1%

---

# 200 Trenchesの記事

200件以上のEdge Delivery Services プロジェクトを完了した後、AdobeのシニアエンジニアであるKiran Murugulla氏とAdobe Experience Manager CloudのアーキテクトであるVarun Mitra氏が、学んだ重要な教訓を共有します。 Core Web Vitalsが実現する、優れた顧客体験をすばやく提供するための秘訣をご紹介します。


>[!VIDEO](https://video.tv.adobe.com/v/3439424/?learn=on&enablevpops)

## コミュニティ議論

Adobe Developers Live コミュニティ [&#x200B; ディスカッション &#x200B;](https://adobe.ly/4fwWvvi)で引き続きディスカッションを行います。

## 重要な留意点

* **パフォーマンスは重要です** パフォーマンス、特にweb ページの速度は、web プロジェクトを成功させるための重要な要素として強調されます。 パフォーマンススコアを100に保つことは主要な目標です。
* **開発プラクティス**
   * GoogleのPageSpeed Insightsを使用して、開発中の継続的なテストを実施。
   * 既に100点を獲得している定型文のコードを使用してプロジェクトを開始し、高いパフォーマンスを維持できます。
   * プル要求（PR）がマージ前にパフォーマンス基準を満たしていることを確認します。
* **主要指標**&#x200B;は、パフォーマンススコアに大きな影響を与えるため、LCP （Largest Contentful Paint）とTBT （Total Blocking Time）の最適化に重点を置いています。
* **リソース管理**
   * フォントやサードパーティのスクリプトなどの必要なリソースをプロジェクトソースに含めます。
   * フォントフォールバックを使用して、読み込み時間を短縮できます。
   * 初期読み込みのパフォーマンスを向上させるために、必須ではないスクリプトの読み込みを遅らせます。
* **画像の最適化**&#x200B;折り返し画像の読み込みを優先し、重要な画像には高優先度のフェッチ設定を使用します。
* **ユーザー事例**
   * ***CNN.com***&#x200B;最適化されたクエリインデックスと、パフォーマンスを向上させるためのGoogle広告の読み込みの遅延。
   * ***Herbert Homes***&#x200B;は、Intersection Observer APIを使用して、ユーザーがスクロールする際にデータを読み込み、パフォーマンスとユーザーエクスペリエンスを向上させました。
* **ベストプラクティス**
   * まず定型文コードから始め、適切に構造化されたマークアップを使用します。
   * 高度なCSS セレクターを活用し、JavaScriptの操作を最小限に抑えます。
   * 特にモバイルで開発を進める場合。
   * コンテンツ制作者は直観的にコンテンツを構造化できます。
* **ツール** Google SheetsやDSAなどのツールを使用して、サイトのパフォーマンススコアを経時的に追跡します。
