---
title: Marketo APIを使用したキャンペーン運用の自動化と合理化
description: ここでは、Marketo APIを利用して、マーケティング業務を効率化する方法を解説します。メールマガジンの作成、プログラムの追跡、重複の結合、プログラムコストの更新、プログラムの複製などの反復作業を自動化し、戦略的な取り組みに注力できるようにする方法を紹介します。
feature: Smart Lists
topic: Integrations, Performance
role: Admin, Developer, User
level: Intermediate, Experienced
doc-type: Event
duration: 4370
last-substantial-update: 2024-11-22T00:00:00Z
jira: KT-16520
exl-id: ff95d1d0-3150-451d-bf45-17e3248689e5
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 1%

---

# Adobe Adobe Marketo Engage Championの詳細 – Marketo APIを使用したキャンペーン運用の自動化と合理化

Adobe Marketoのユーザーとしての役割の1つは、マーケティング部門が実施するマーケティング施策をサポートすることです。 つまり、コンテンツを制作する際には、次のような反復的な作業を行う必要があります。

* メールニュースレター
* アトリビューション追跡プログラム
* コンテンツパフォーマンス追跡プログラム
* 重複の結合
* プログラム期間コストの更新
* 複製プログラム

この記事では、Marketo APIの概要、利点、導入方法を解説します。

>[!VIDEO](https://video.tv.adobe.com/v/3440396/?learn=on&enablevpops)

## 重要な留意点

* **Focus** Marketo APIを使用したキャンペーンオペレーションの自動化と合理化に焦点を当てたセッションです。
* **APIの重要性** APIは、反復的なタスクを自動化し、システムが通信できるようにし、時間とコストを節約するために重要です。APIの基本&#x200B;**Get リクエストとPost リクエストの違い、およびそれらの機能を含む* &#x200B;** APIの概要を説明します。

### ユースケース

* **プログラムの一括作成** Python スクリプトを使用したプログラムの複製、トークンの更新、スマートキャンペーンのアクティブ化。 &#x200B;
* **オンデマンドプログラムの作成** Zapierを使用して、UTM パラメーターの生成やトラッキング用* **JIRA チケットの作成など、フォーム送信に基づいてMarketo プログラムの作成を自動化します。
* **API管理**&#x200B;異なる統合用に個別のローンチポイントサービスを作成したり、API呼び出しの使用状況を監視したりするなど、APIの使用状況を管理する際のヒント。API リクエストのテストにPostmanを、Python コードの生成にChatGPTなどのツールを使用する場合のツールと* **リソース**&#x200B;の推奨事項。
* **その他のユースケース** データの変更の元に戻す、重複排除、MarketoとAIの接続など、Marketo APIのその他の潜在的なユースケースに関する記載。
