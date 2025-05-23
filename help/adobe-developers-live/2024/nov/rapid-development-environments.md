---
title: Adobe Experience Managerの迅速な開発環境
description: Adobeの新しい SDK を使用すると、クラウド環境での迅速な開発とデプロイメントが容易になり、デプロイメント時間が大幅に短縮され、クイックアップデート、ライブログ、高度な設定オプションがサポートされます（DevOps Life 2024 を参照）。
feature: Developer Tools
topic: Development
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2427
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16570
source-git-commit: 07d4174b0d89ba2c417866e76ae72f015b91b03a
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---


# Adobe Experience Managerの迅速な開発環境

迅速な開発環境（RDE）と更新された開発者コンソールのベストプラクティスについて説明します。 Adobeのソフトウェア開発エンジニアである Natalia Angulo Herrera とAdobeのソフトウェア開発エンジニアである Remo Liechti が、移行の課題、AIO CLI の設定、導入、テスト、ログ記録、設定管理について説明し、よりスムーズなAdobe Experience Managerワークフローを実現します。

>[!VIDEO](https://video.tv.adobe.com/v/3440397/?learn=on&enablevpops)


## コミュニティ ディスカッション

Adobe Developers Live コミュニティで会話を続けます [ ディスカッション ](https://adobe.ly/3UJluDo)。

## 重要ポイント

* **DevOps Life 2024 の概要** このセッションは、Adobeの Natalia と Remo が主催し、迅速な開発環境に焦点を当てています。
* **問題の説明** ローカルでは正常に動作しているが、クラウドにデプロイすると失敗するローカル開発環境の課題。
* **解決策** 迅速な開発とデプロイメントを容易にするためにクラウドに新しい SDK を作成し、30 分から数秒または数分の時間を短縮します。
* **デプロイメントプロセス** 新しい環境では、新しい API および CLI プラグインを使用して迅速な更新と検証が可能になり、フィードバックとデプロイメントを迅速に行うことができます。
* **インフラストラクチャの違い** クラウド環境では、高可用性を備えていない 1 つのオーサーインスタンスとパブリッシュインスタンスを使用し、MongoDB は使用しません。
* **設定と使用** 開発者は、npm とAdobe IO CLI を使用して、クラウドインターフェイスを通じて迅速な開発環境を設定できます。
* **基本コマンド** 主なコマンドには、io amd —help、io login、io status、io install、io history、io delete、io reset などがあります。
* **ログとデバッグ** 新しい環境では、io am や d ログなどのコマンドを使用して、再デプロイメントなしでライブログとログレベルの変更をサポートしています。
* **詳細なトピック** フロントエンドパッケージと設定パイプラインのサポートで、デプロイメントとイテレーションを迅速に行えます。
* **今後の機能** コンテンツを失うことなく、環境のリセットと自動更新を容易にするスナップショット機能の導入を予定しています。
* **Q&amp;A とフィードバック** セッションでは、Discord チャネルに参加して開発チームとのライブインタラクションやフィードバックを行うことを推奨しています。