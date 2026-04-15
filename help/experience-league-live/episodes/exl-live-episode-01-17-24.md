---
title: Adobe Analyticsのデータと分析をCustomer Journey Analyticsに取り込み
description: Adobe AnalyticsからAdobe Customer Journey Analyticsに分析データを移行する際に、新しい自動化プロセスがどのように役立つかをご覧ください。
jira: KT-14746
solution: Analytics,Customer Journey Analytics
feature: Experience Cloud Integration
topic: Integrations, Migration, Administration
event-cta-url-live: https://www.youtube.com/watch?v=BkAjaMPgpgE
event-cta-url-reg: https://engage.adobe.com/ExpLeagueLive-240117.html
event-start-time: 2024-01-17 10:00-7
event-guests: Doug Moore,Eric Matisoff,Bryan Skelton
exl-id: 2c2136a9-0b40-4a0a-907d-5af181568073
duration: 3655
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 6%

---

# Adobe Analyticsのデータと分析をCustomer Journey Analyticsに取り込み

Bryan、Eric、Dougが、CJAを利用して、すぐに使い始める方法を解説します。 自動プロセスを使用して、Adobe Analytics から CJA にデータと分析結果を移行する方法と、プロセス中に考慮すべき潜在的な問題について説明します。 その過程で、楽しいヒントやコツを十分に用意しましょう。

>[!VIDEO](https://video.tv.adobe.com/v/3426778/?quality=12&learn=on)

>[!BEGINSHADEBOX  「質問がありますか？」 ]

[Experience League コミュニティフォーラムのディスカッション ](https://experienceleaguecommunities.adobe.com/t5/adobe-analytics-discussions/experience-league-live-post-session-discussion-bringing-your/m-p/646093#M3582)に関するディスカッションを続けます。

>[!ENDSHADEBOX]

## 重要な留意点

* Adobe AnalyticsからCustomer Journey Analyticsにデータを取り込むには、Analytics Data Connector （ADC）とWeb SDKの2つの方法があります。
* ADCでは、レポートスイートのデータをAdobe Experience Platformにコピーして分析し、Web SDKではAdobe Experience Platformに直接データを送信できます。
* Customer Journey Analyticsのデータビューでは、プラットフォームに取り込まれるデータをカスタマイズして分析できます。
* データビューには、遡及変更、カスタマイズ用の派生フィールド、詳細レベルでのデータのフィルタリングや分析などの強力な機能が用意されています。
* Customer Journey Analyticsのコネクションを使用すると、異なるデータセットの結合が可能になり、複数のデータソースを1か所で分析できます。
* データのアクセスと分析に対する適切なガバナンスと制御を確保するために、データ表示と接続は戦略的かつ慎重に使用する必要があります。
* Adobe Analytics管理者がプロジェクトをCJAに移行できる「コンポーネント移行」という新しいツールがあります。
* プロジェクトを移行すると、テーブル内のすべてのコンポーネントと、適用されたセグメントや計算指標がCJAに移動されます。
* CJAに存在しないコンポーネントを、catch-all フィールドまたは派生フィールドを使用してマッピングできるマッピングプロセスがあります。
* CJAに存在しない要素のキャッチオールを作成してから、対象プロジェクトで編集することをお勧めします。
* 以前は、CJAに移行する際に、計算指標とセグメントを再作成する必要があると考えられていましたが、現在では移行するオプションがあります。
* 計算された指標とセグメントを確実に移行に含めるには、Adobe Analyticsのテーブルまたはビジュアライゼーションに適用する必要があります。

