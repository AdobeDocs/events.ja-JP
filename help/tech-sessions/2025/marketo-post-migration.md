---
title: Adobe Admin ConsoleへのMarketoの移行 – （移行後）
description: Adobe Admin ConsoleでMarketoのユーザー管理を一元化。 役割（システム管理、製品管理、プロファイル管理、サポート管理者）およびID タイプ（Adobe、エンタープライズ管理、Federated ID管理）の管理。 シングルサインオン用にSSLを設定し、ユーザー管理を処理し、証明書を3年ごとに更新します。 ログインの問題などの一般的な問題に対処し、ディレクトリの信頼を利用して統合されたエクスペリエンスを実現します。 大規模なユーザーのコンバージョンを500件のバッチに分割します。 AdobeのExperience League ページのセッション録画にアクセスします。
solution: Marketo Engage
feature: Programs, Reporting
topic: Security, Migration, Certification
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3194
last-substantial-update: 2025-03-14T00:00:00Z
jira: KT-17534
exl-id: d9ccabf4-5eff-4e07-a7ff-6509bb6ff3c8
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Adobe Admin ConsoleへのMarketoの移行 – 移行後


MarketoをAdobe Admin Consoleに移行した後、次の手順は何ですか？ Adobeのカスタマーエクスペリエンス&amp;ID チームが提供する移行後のウェビナーは、新しい環境で自信を持ってナビゲートできるように設計されています。

アドビのエキスパートのテクニカルサポートエンジニアが、新しい設定を最大限に活用できるように、主な機能、ベストプラクティス、一般的なトラブルシューティングのヒントを説明します。

得られるものは何か，

* Marketoのユーザー向けAdmin Consoleの基本機能ツアー
* ユーザー、権限、設定の管理に関するベストプラクティス
* Adobeのエキスパートによる移行後の一般的な質問に対する回答

アドビのエキスパートが、お客様の質問に答え、Admin Console体験の最適化を支援するソリューションを提供します。 最後に、ライブ Q&amp;Aを行い、実用的なインサイトと新しいプラットフォームについてより深く理解したところで終わります。

ワークフローを強化し、Marketoへの移行を最大限に活用するチャンスをお見逃しなく！

>[!VIDEO](https://video.tv.adobe.com/v/3451635/?learn=on&enablevpops)

## 重要な留意点

* **Admin Consoleの目的**&#x200B;他のAdobe製品と連携して、Marketo ユーザー、管理者、IDを一元管理します。

* **Admin Consoleの役割**

   * **システム管理者**&#x200B;完全アクセス
   * **製品管理者**&#x200B;は特定の製品を管理します
   * **プロファイル管理者**&#x200B;は特定のプロファイルを管理します
   * **サポート管理者**&#x200B;がサポートチケットを送信

* **ID タイプ**

   * **Adobe ID**&#x200B;個人用アカウント
   * **Enterprise ID**&#x200B;会社がSSLなしで管理
   * **Federated ID** シングルサインオン （SSL）

* **シングルサインオン （SSL）**&#x200B;には、ディレクトリの設定、ドメインの追加、メタデータファイルのアップロードが必要です。

* **User Management** Admin Consoleを使用してユーザーと管理者を追加または削除します。CSV ファイルを使用してAdobe IDをFederated IDに変換します。

* **サポートプロセス** Experience League ディレクトリを介してケースを送信します。「サポート管理者」の役割が必要です。

* **一般的な問題**

   * 広告ブロッカー、ID タイプの不一致、SSL エラーによるログインの問題。
   * パスワードまたはネットワークパスワードの問題を忘れた。

* **証明書の更新** SSL証明書は、Admin Consoleを介して3年ごとに更新する必要があります。

* **ユーザーグループ**&#x200B;特定のツールのユーザーを整理します。ローカルで管理することも、Active Directoryと同期することもできます。

* **移行後の考慮事項**&#x200B;製品間で一貫したID タイプを確保します。統合されたユーザーエクスペリエンスには、ディレクトリの信頼を使用します。

* **大規模なユーザーベース管理** ユーザーのコンバージョンを500のバッチに分割して、効率を高めます。
