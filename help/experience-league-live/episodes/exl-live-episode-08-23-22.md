---
title: エキスパートに質問する – タグ（Launch）の便利な拡張機能を使用して、Web SDK を大幅に請求できます
description: 実装を新しいAdobe Web SDK に移行することを考えていますか？  データ収集を次のレベルに引き上げるのに役立つ、Adobeタグライブラリのお気に入りの拡張機能をいくつか実行します。
solution: Data Collection, Experience Platform
feature: Tags
kt: 10528
event-start-time: 2022-08-23 09:00-7
event-guests: Rudi Shumpert,Jeff Chasin,Eric Matisoff
exl-id: 5ef987f4-37f5-473f-b9f2-1598b7e655ba
duration: 3833
source-git-commit: 0b2f63198af8767f24783dbafd244c9398c24f33
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 0%

---

# エキスパートに質問する：Web SDK の超充電に役立つ、タグ（Launch）の便利な拡張機能

実装を新しいAdobe Web SDK に移行することを考えていますか？  データ収集を次のレベルに引き上げるのに役立つ、Adobeタグライブラリのお気に入りの拡張機能をいくつか実行します。

>[!VIDEO](https://video.tv.adobe.com/v/346610/?quality=12&learn=on)

## 番組からの質問とコメント

### Evolytics の Data Element Assistant 拡張機能

<br> 
**質問：** データセキュリティの観点から見ると、Evolytics はサードパーティ製の拡張機能なので、安全に使用できますか？

**回答：** はい。 必要に応じて、拡張機能コードを確認できます。また、日付を保存せず、変換のみを行います。

<br> 

**質問：** これはAdobe ECID も取り込みますか？

**回答：** AdobeECID は、その拡張機能内ではキャプチャされません。 この拡張機能は、（特に）追加の匿名識別子を作成するためのものです。

**回答：** ただし、Adobe ECID は他の方法で取得することもできます。 ここではチャットでリンクを共有できないので、ExL のメモとTwitterを使用して共有します。

<br> 

**質問：** ハッシュ機能は、SHA-256 などの様々なハッシュ手法を提供し、公開鍵と秘密鍵を提供しますか。

**回答：** うん！ デフォルトは SHA-256 です

<br> 

### 一般的な質問とコメント：

<br> 

**質問：** 拡張子のソースファイルをダウンロードするには、何をクリックしますか？ それは「3 ドットメニュー」ですか。

**回答：** はい！ 3 つのドット、「ソースをダウンロード」（カタログ表示から）の順に選択

<br> 

**コメント：** 拡張機能で私が本当に掘り下げていることの 1 つは、それらの時間節約の側面です。 彼らの多くはあなたのことを行います *可能性のある* カスタムコードを使用しますが、拡張機能を使用すると、そのコードを記述する必要がなくなります。

**返信：** 右。 そして、毎回車輪を作り直すことなく繰り返し可能です。

<br> 

**質問：** Analytics プラグインはどのようにサポートされたり、Web SDK 実装に置き換えられたりしますか？

**回答：** Workspace とAdobeタグの柔軟性が向上したことで、最近では多くの Analytics プラグインが実際には必要なくなりました。 ただし、そうでない実装は、Web SDK で使用するために積極的に移行されています。

<br> 

**質問：** Web SDK を使用した Activity Map トラッキングに関する開発はありますか？

**回答：** Activity Mapが Web SDK でのサポートに向けて積極的に取り組んでいることをお知らせします

<br> 

**質問：** Adobe Edge Network にアクセスしてイベントを管理してからエンドポイントに転送することはできますか？ Launch でも実行できると思いますが、将来的にはサーバーでも実行できますか？

**回答：** はい！ これは、お客様がアドビの任意のReal-Time CDP製品（Real-Time CDP Connections、Prime または Ultimate）を通じて購入できるイベント転送機能を通じて可能です。

**回答：** RTCDP Connections （イベント転送）は、アドビ以外の宛先に送信する前に、より詳細な制御を行う機能を提供します。

**回答：** 詳しくは、その他の ExL Live ビデオをご覧ください [この 1](exl-live-episode-06-23-22.md)）に設定します。

<br> 

**コメント：** 私のお気に入りの拡張機能の 1 つに対するクイックコール：マッピングテーブル拡張機能があり、データ要素のテーブルを読み取ることができます「この値がこれの場合、そのように設定します」。

**返信：** 彼らが提供する柔軟性は非常に印象的です。 また、企業は独自のプライベート拡張機能を作成することもできます（選択した場合）。

<br> 

**質問：** 都市や天気などの CRM の個人データを示しましたが、個人の応答はどこに保存されていますか？

**回答：** 応答は、イベント転送プロパティ内のルールをトリガーする一意の各イベントに保存され、その特定のイベントでのみ使用されます。

<br> 

このトピックに関するディスカッションを [Experience Leagueコミュニティのディスカッション](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-platform/experience-league-live-post-session-discussion-useful-extensions/m-p/542620#M240).
<br> 

## このデータ収集シリーズのその他のExperience Leagueライブセッション

* [エキスパートに質問 – Web SDK の基本](exl-live-episode-05-26-22.md)
* [エキスパートへの質問 – RTCDP Connections](exl-live-episode-06-23-22.md)
* [エキスパートに質問する – データストリームとデータ準備](exl-live-episode-07-21-22.md)

