---
title: Adobe Analyticsのデータと分析のCustomer Journey Analytics化
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
source-git-commit: 0b2f63198af8767f24783dbafd244c9398c24f33
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Adobe Analyticsのデータと分析のCustomer Journey Analytics化

Bryan、Eric、Doug が、Customer Journey Analytics（CJA）をすぐに使い始める方法について説明します。 自動プロセスを使用して、Adobe Analyticsから CJA にデータと分析を移行する方法と、プロセス中に考慮すべき潜在的な問題について説明します。 そしてもちろん、彼らは途中で楽しいヒントやトリックの健康的な線量を持っているでしょう。

>[!VIDEO](https://video.tv.adobe.com/v/3426778/?quality=12&learn=on)

>[!BEGINSHADEBOX 「ご質問がある場合」]

～について議論を続ける [Experience Leagueコミュニティフォーラムのディスカッション](https://experienceleaguecommunities.adobe.com/t5/adobe-analytics-discussions/experience-league-live-post-session-discussion-bringing-your/m-p/646093#M3582).

>[!ENDSHADEBOX]

## 重要ポイント

* Adobe AnalyticsからデータをCustomer Journey Analyticsに取り込むには、Analytics Data Connector （ADC）と Web SDK の 2 つの方法があります。
* ADC を使用すると、レポートスイートのデータを分析用にAdobe Experience Platformにコピーしながら、Web SDK はデータをAdobe Experience Platformに直接送信できます。
* Customer Journey Analyticsのデータビューを使用すると、プラットフォームに取り込むデータをカスタマイズおよび分析できます。
* データビューは、遡及的変更、カスタマイズ用の派生フィールド、詳細なレベルでデータをフィルタリングおよび分析する機能などの強力な機能を提供します。
* Customer Journey Analytics内の接続を使用すると、異なるデータセットを結合でき、複数のデータソースを 1 か所で分析できます。
* データのビューと接続は、データのアクセスと分析に対する適切なガバナンスと制御を確保するために、戦略的かつ慎重に使用する必要があります。
* Adobe Analytics管理者がプロジェクトを CGA に移行できる「コンポーネント移行」という新しいツールがあります。
* プロジェクトを移行すると、テーブル内のすべてのコンポーネントと、適用されたセグメントや計算指標は CGA に移行されます。
* CGA に存在しないコンポーネントを、キャッチオールまたは派生フィールドを使用してマッピングできるマッピングプロセスがあります。
* CGA に存在しない要素にすべてを取得して、宛先プロジェクトで編集することをお勧めします。
* 以前は、CGA への移行時に計算指標とセグメントを再作成する必要があると考えられていましたが、現在は移行するオプションがあります。
* 計算指標とセグメントが確実に移行に含まれるようにするには、Adobe Analyticsのテーブルまたはビジュアライゼーションに計算指標とセグメントを適用する必要があります。

