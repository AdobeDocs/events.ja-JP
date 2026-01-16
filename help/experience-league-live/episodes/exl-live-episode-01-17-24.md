---
title: Adobe Analytics データと分析のCustomer Journey Analyticsへの取り込み
description: 新しい自動プロセスが、分析とデータをAdobe AnalyticsからAdobe Customer Journey Analyticsに移行するのにどのように役立つかについて説明します。
jira: KT-14746
solution: Analytics,Customer Journey Analytics
feature: Experience Cloud Integration
event-cta-url-live: https://www.youtube.com/watch?v=BkAjaMPgpgE
event-cta-url-reg: https://engage.adobe.com/ExpLeagueLive-240117.html
event-start-time: 2024-01-17 10:00-7
event-guests: Doug Moore,Eric Matisoff,Bryan Skelton
exl-id: 2c2136a9-0b40-4a0a-907d-5af181568073
duration: 3655
source-git-commit: a004d7aa2c01ccd1d4d65749c4aa0440290f8023
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Adobe Analytics データと分析のCustomer Journey Analyticsへの取り込み

Bryan、Eric、Doug が、Customer Journey Analytics（CJA）をすぐに使い始める方法について説明します。 自動プロセスを使用して、Adobe AnalyticsからCJAにデータと分析を移動する方法と、プロセス中に考慮すべき問題点について説明します。 そしてもちろん、彼らは途中で楽しいヒントやトリックの健康的な線量を持っているでしょう。

>[!VIDEO](https://video.tv.adobe.com/v/3426778/?quality=12&learn=on)

>[!BEGINSHADEBOX  「ご質問がある場合」 ]

[Experience League コミュニティフォーラムのディスカッション &#x200B;](https://experienceleaguecommunities.adobe.com/t5/adobe-analytics-discussions/experience-league-live-post-session-discussion-bringing-your/m-p/646093?profile.language=ja#M3582) でディスカッションを続行します。

>[!ENDSHADEBOX]

## 重要な留意点

* Adobe AnalyticsからCustomer Journey Analyticsにデータを取り込むには、Analytics Data Connector （ADC）と Web SDKの 2 つの方法があります。
* ADC を使用すると、分析のためにレポートスイートのデータをAdobe Experience Platformにコピーしながら、Web SDKはデータをAdobe Experience Platformに直接送信できます。
* Customer Journey Analyticsのデータビューを使用すると、プラットフォームに取り込むデータをカスタマイズおよび分析できます。
* データビューは、遡及的変更、カスタマイズ用の派生フィールド、詳細なレベルでデータをフィルタリングおよび分析する機能などの強力な機能を提供します。
* Customer Journey Analyticsの接続を使用すると、異なるデータセットを結合でき、複数のデータソースを 1 か所で分析できます。
* データのビューと接続は、データのアクセスと分析に対する適切なガバナンスと制御を確保するために、戦略的かつ慎重に使用する必要があります。
* Adobe Analytics管理者がプロジェクトをCJAに移行できる「コンポーネント移行」という新しいツールがあります。
* プロジェクトを移行すると、テーブル内のすべてのコンポーネントと、適用されたセグメントや計算指標は、CJAに移動されます。
* マッピングプロセスには、CJAに存在しないコンポーネントを、キャッチオールまたは派生フィールドを使用してマッピングできるものがあります。
* CJAに存在しない要素にすべてを取得して、出力先プロジェクトで編集することをお勧めします。
* 以前は、CJAへの移行時に計算指標とセグメントを再作成する必要があると考えられていましたが、現在は指標とセグメントを移行するオプションがあります。
* 計算指標とセグメントが確実に移行に含まれるようにするには、Adobe Analyticsのテーブルまたはビジュアライゼーションに計算指標とセグメントを適用する必要があります。

