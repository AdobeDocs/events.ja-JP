---
title: Cloud Managerによる DevOps の合理化
description: AMP Cloud ManagerのAdobeの新しい「Bring Your Own Git」機能を使用すると、外部 Git リポジトリを直接統合でき、コード品質の初期チェックのための左シフト戦略に対応し、効率性と適応性を向上させることで、デプロイメントワークフローを最適化できます。
solution: Experience Manager, Experience Manager Cloud Manager
feature: Git Repositories, CI-CD Pipeline
topic: Integrations
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1034
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16547
source-git-commit: a5b6c2c3150fcc98686fe74d68f186bfe4e1befa
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 0%

---


# Cloud Managerによる DevOps の合理化

エクスペリエンスを大規模に提供するには、効率的な DevOps プラクティスが不可欠です。 Adobeのソフトウェア開発エンジニアである Adrian Tanase が、Adobe Experience Manager Cloud Managerでデプロイメントワークフローを合理化し、自動化を強化し、継続的インテグレーションと継続的デリバリー（CI/CD）をサポートする方法について説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3439904/?learn=on&enablevpops)

## コミュニティ ディスカッション

Adobe Developers Live コミュニティで会話を続けます [ ディスカッション ](https://adobe.ly/3Ywf7Vm)。

## 重要ポイント

* **新機能の紹介** Adobeの Adriana Clayton は、AMP Cloud Managerに「Bring Your Own Git」という新機能を導入しました。
* **機能の目的** この機能は、デプロイメントワークフローを最適化するように設計されており、より速く、より効率的で、好みのベンダーに適応できます。
* **対処された課題** この機能は、外部 Git リポジトリとAdobe Git リポジトリの同期の複雑さに対処するもので、デプロイメントプロセスに追加の手順と時間が必要になります。
* **提供されるソリューション** 「独自の Git を取り込む」を使用すると、プライベートおよびパブリックの外部 Git リポジトリをCloud Manager パイプラインに直接接続でき、コードの変更と、コードのマージ前のアクションの実行を即座に認識できます。
* **左シフト戦略** 統合は、左シフト戦略をサポートしており、開発プロセスの早い段階でコード品質チェックを実行でき、開発者にタイムリーなフィードバックを提供できます。
* **デモと検証** GitHub および Bitbucket リポジトリの手順など、リポジトリを統合し、Cloud Managerを使用して検証する方法を示すデモが提供されました。
* **お客様への影響** 一般提供開始以降、130 を超えるお客様がリポジトリにオンボーディングし、コード品質の問題を伴う 2500 を超えるプルリクエストが実稼動環境に到達するのを防ぎました。
* **今後の機能強化** この機能を拡張して GitLab および Bitbucket に直接レポートを含めたり、エッジ配信サービスに「Bring Your Own Git」を拡張して柔軟性を高めたりする予定です。
* **フィードバックの励まし** お客様には、フィードバックを提供し、GitHub 以外のリポジトリの早期導入段階に参加することをお勧めします。
