---
title: Adobe Analyticsのデータと分析をCustomer Journey Analyticsに取り込む
description: 新しい自動プロセスが、分析やデータをAdobe AnalyticsからAdobe Customer Journey Analyticsに移行する際に役立つ理由を説明します。
jira: KT-14746
thumbnail: https://video.tv.adobe.com/v/3426778?format=jpeg
event-cta-url-live: https://www.youtube.com/watch?v=BkAjaMPgpgE
event-cta-url-reg: https://engage.adobe.com/ExpLeagueLive-240117.html
event-start-time: 2024-01-17 10:00-7
event-guests: Doug Moore,Eric Matisoff,Bryan Skelton
exl-id: 2c2136a9-0b40-4a0a-907d-5af181568073
duration: 3655
source-git-commit: 604f85ddc402ed248678782412efe4f2e5988ab4
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Adobe Analyticsのデータと分析をCustomer Journey Analyticsに取り込む

Customer Journey Analytics(CJA) との迅速な移行方法について話し合いながら、ブライアン、エリック、ダグに加わりましょう。 自動化されたプロセスを使用して、Adobe Analyticsから CJA にデータと分析を移動する方法、およびプロセスの過程で考慮すべき問題について学びます。 もちろん彼らは楽しいヒントやコツを楽しみながら進むのです

>[!VIDEO](https://video.tv.adobe.com/v/3426778/?quality=12&learn=on)

>[!BEGINSHADEBOX 「ご質問は？」]

次に関するディスカッションを続行します： [Experience Leagueコミュニティフォーラムディスカッション](https://experienceleaguecommunities.adobe.com/t5/adobe-analytics-discussions/experience-league-live-post-session-discussion-bringing-your/m-p/646093#M3582).

>[!ENDSHADEBOX]

## 重要ポイント

* Adobe AnalyticsからデータをCustomer Journey Analyticsに取り込む方法は、Analytics Data Connector(ADC) と Web SDK の 2 つです。
* ADC を使用すると、レポートスイートのデータを分析用にAdobe Experience Platformにコピーでき、Web SDK がAdobe Experience Platformに直接データを送信できます。
* Customer Journey Analyticsのデータビューは、プラットフォームに取り込むデータをカスタマイズし、分析する方法を提供します。
* データビューは、遡及的な変更、カスタマイズのための派生フィールド、詳細なレベルでのデータのフィルタリングと分析機能などの強力な機能を提供します。
* Customer Journey Analytics内の接続を使用すると、異なるデータセットを結合でき、複数のデータソースを 1 か所で分析できます。
* データのアクセスと分析を適切なガバナンスと制御するために、データビューと接続は戦略的かつ慎重に使用する必要があります。
* Adobe Analytics管理者がプロジェクトを CGA に移行できる、「コンポーネントの移行」という新しいツールが追加されました。
* プロジェクトを移行する際、テーブル内のすべてのコンポーネントと、適用されたセグメントまたは計算指標が CGA に移行されます。
* マッピングプロセスでは、CGA に存在しないコンポーネントは、包括的フィールドまたは派生フィールドを使用してマッピングできます。
* CGA に存在しない要素の包括的な要素を作成して、宛先プロジェクトで編集することをお勧めします。
* 以前は、CGA への移行時に計算指標とセグメントを再作成する必要があると考えられていましたが、現在は、計算指標とセグメントを移行するオプションが用意されていました。
* 計算指標とセグメントを移行に含めるには、Adobe Analyticsのテーブルまたはビジュアライゼーションに適用する必要があります。
