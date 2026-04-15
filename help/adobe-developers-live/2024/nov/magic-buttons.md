---
title: 魔法のボタンとその構築方法
description: AdobeのUI拡張性により、ワークフローとユーザーエクスペリエンスを強化します。Adobe App Builderによるカスタム統合が可能で、「魔法のボタン」を使って複雑なタスクを簡素化し、エンタープライズシステムとのシームレスな統合をサポートします。将来的にはより多くのAdobe サービスに拡張する予定です。
solution: Experience Manager
feature: Developer Tools, Authoring
topic: Development
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1226
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16548
exl-id: 9dafd048-8b3a-444f-bf0e-d49f76ae7054
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# 魔法のボタンとその構築方法

Adobe Experience ManagerのUIを拡張して、反復的なコンテンツタスクを自動化する方法をご確認ください。 AdobeのシニアプロダクトマネージャーであるSarah Xu氏は、ビジネスニーズに合わせてコンテンツフラグメント拡張機能やユニバーサルエディターをカスタマイズした実例を紹介しています。


>[!VIDEO](https://video.tv.adobe.com/v/3440037/?learn=on&enablevpops)

## コミュニティ議論

Adobe Developers Live コミュニティ [ ディスカッション ](https://adobe.ly/3Ywf6kg)で引き続きディスカッションを行います。

## 重要な留意点

* Adobeのプロダクトマネージャーである&#x200B;**UI Extensibility** Sarahが、開発者がカスタム統合と拡張機能を作成してワークフローとユーザーエクスペリエンスを向上できるようにするUI拡張性の概念について説明します。
* **魔法のボタン**&#x200B;複雑なワークフローを単一のアクションに単純化し、効率を高め、フラストレーションを軽減する「魔法のボタン」のアイデアが導入されました。
* **拡張ポイント**&#x200B;これらは、カスタマイズを行うことができるアプリケーション内の事前定義済みの領域です。 エクステンションは、これらのポイントの予想される形状と色に一致する必要があります。
* **Adobe App Builder**&#x200B;これは、AEM（Adobe Experience Manager）などのAdobe ソリューションと統合するUI拡張機能を構築するためのフレームワークです。 フロントエンドとバックエンドの両方のコンポーネントをサポートしています。
* **配布**&#x200B;拡張機能は、組織内で非公開で配布するか、Adobe Exchange Marketplaceを通じて公開できます。
* **Extension Manager**&#x200B;このツールを使用すると、AEM環境内での拡張機能の表示と機能を管理できます。
* **メリット** UI拡張機能により、コンテキストの切り替えが最小限になり、効率が向上し、他のエンタープライズシステムとのシームレスな統合が可能になります。 Adobeでホストされ、最新のテクノロジースタックを使用し、AEMとは別に管理できます。
* **ユースケース**&#x200B;の例には、ワークフローの自動化、カスタムウィジェット、データの同期、カスタムダッシュボードなどがあります。 具体的な例として、生成AI コンテンツアシスタント、ローカライゼーションツール、自動車モデルピッカーが挙げられている。
* **今後の開発** Adobeでは、UIの拡張性をWorkfront、Content Hub、Gen Studioなどのより多くのサービスに拡張しています。
* **リソース** ドキュメントと詳細な学習リソースは、提供されたQR コードから入手できます。
