---
title: Workfront API と Fusion のナビゲーションが変更され、複数選択フィールドを簡単にナビゲートできる
description: 複数選択のフィールドのアップデート、イベント購読のバージョン管理、重大な変更を防ぐための戦略など、今後のAdobe Workfront API および Fusion の変更について説明します。
feature: Workfront API, Workfront Fusion, Workfront Integrations and Apps
topic: Integrations
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3172
last-substantial-update: 2025-08-08T00:00:00Z
jira: KT-18631
source-git-commit: 6225f36c5d26ecca5ebc2aca24a2d592a3279570
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---


# Workfront API と Fusion のナビゲーションが変更され、複数選択フィールドを簡単にナビゲートできる

このワークショップは 2025 年 6 月 25 日（PT）に録画され、Andy Hess が特集されて、Workfront API と Fusion の今後の変更点について説明しました。

>[!VIDEO](https://video.tv.adobe.com/v/3469978/?learn=on&enablevpops)

## リソース

オンデマンド録画に加えて、スライドデッキとその他のリソースも含まれています。
* [ スライドデッキPDF](https://workfront-experience.s3.us-west-2.amazonaws.com/Training/Guides/Customer+Success+at+Scale/Navigating+the+API+and+Fusion+Changes+for+Multi-Select+Fields+with+Ease+062425.pdf)
* Adobe Software Development Team と提携して開催されたイベントが 5 月初旬に Event Subscriptions の変更で配信されました。この分野について詳しくは、[[ イベントのフォローアップ ] Event Subscriptions V2 のアップグレード中に Fusion のシナリオを維持する ] を参照してください &rbrack;(https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/event-follow-up-preserving-your-fusion-scenarios-during-the/m-p/754182?profile.language=ja#M4041)

## 主な留意点とリソース

* Workfront API の複数選択フィールドに対する変更が、文字列と配列が混在する応答ではなく、一貫性のある JSON 配列形式を確実に使用できるようにするため、バージョン 21 （2025 年 10 月）で追加されました。
* イベント購読のバージョン管理が導入されました。バージョン 2 は常に複数選択フィールドを配列として返しますが、バージョン 1 は現在の一貫性のない動作を維持します
* 新しいイベント購読は、自動的にデフォルトでバージョン 2 にアップグレードされます。すべての購読は、2026 年 1 月中旬に自動的にバージョン 2 にアップグレードされます
* 新しいWorkfront コネクタバージョンは、モジュールマッピングを保持し重大な変更を防ぐための手動アップグレードプロセスとともに、今年後半にリリースされる予定です
* Fusion AI アシスタントは現在利用可能ですが、署名された AI 契約と適切なライセンス設定が必要です。 ご質問がある場合や、その他の情報に興味がある場合は、担当のアカウントマネージャーにお問い合わせください。 [Fusion での AI の使用に関する詳細 ](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/manage-scenarios/fusion-ai-assistant)
* [ 現在使用可能なWorkfront Fusion テンプレート ](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/create-and-manage-templates/currently-available-fusion-templates)
* [Fusion テンプレートの呼び出し ](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/call-for-fusion-template-ideas/m-p/732085?profile.language=ja#M3686) – 新しい Fusion テンプレートの提案がある場合は、ここに追加します。 チームがアイデアを引き出すのはこの場所です  

フォローアップの質問がある場合は、この [Experience League Community Post](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/event-follow-up-navigating-the-workfront-api-and-fusion-changes/td-p/761253?profile.language=ja) に返信してください。 

今後のカスタマーサクセスワークショップでお会いできるのを楽しみにしています。  完全なリストについては、Experience Leagueの [Workfront イベント ](https://experienceleague.adobe.com/events/?lang=ja&filters=Workfront) を確認し、登録してください。