---
title: エキスパートに質問 – 品質とエンゲージメントの評価
description: 品質とエンゲージメントに関する質問に回答するレポートの作成方法を説明します。 このウェビナーは 2019 年 11 月 13 日（PT）に録画されました。
doc-type: feature video
team: Technical Marketing
kt: 9914
exl-id: 76a8e418-71c7-414a-9938-e64e4e73c184
duration: 3980
source-git-commit: 9a297cda953d4414131657f9ac84580aea0eabeb
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 0%

---

# エキスパートに質問 – 品質とエンゲージメントの評価

品質とエンゲージメントに関する質問に回答するレポートの作成方法を説明します。 このウェビナーは 2019 年 11 月 13 日（PT）に録画されました。

>[!VIDEO](https://video.tv.adobe.com/v/341120/?quality=12)

## Q&amp;A

**質問**

フィルタリングに使用できるフィールドがいくつかありますが、それらを使用してグループ化しようとすると使用できません。 一貫したオプションを提供するために取り組んでいますか？

**回答**

レポートツールでは、動的フィールド、またはチェックボックスフィールドのように一度に複数の場所を選択できるフィールドでグループ化することはできません。 選択肢が多数ある場合でも、グループ化できるのは 1 つの値を持つフィールドのみです。

チェックボックスでフィルタリングして表示することはできますが、グループ化することはできません。

**質問**

担当業務のイテレーションの例では、プライマリを太字で表示できますか？

**回答**

このイテレーションでは、プライマリ担当業務を特定できます。 valueexpression でこれを行う必要がありますが、HTMLコードは valueexpression では認識されません。 したがって、この役割をプライマリとして識別する別の方法を考え出す必要があります。 このコードでは、プライマリ役割名の前後に「**」を付けます。 試してみて、気に入ったところを確認してください。

```
displayname=All Job Roles 
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("**",{role}.{name},"**"),{role}. {name})
valueformat=HTML
```

次のようなリストが表示されます。

```
Support Engineer 
QA Engineer 
**Designer**
```

ここで、Designerはこのユーザーの主要な役割です。

**質問**

こんにちはさん。 私は、記事がライフサイクルのどの段階にあるかを追跡する、エディトリアルチーム向けのワークフローを作っています（初期執筆/部門のレビュー/最終編集/公開）。 この会社では、現在、マイルストーンまたはタスクを簡単に確認したいと考えています。 私が受け取るフィードバックは、標準のマイルストーンビュー（赤または緑のシェーディング）では「ビジーで複雑」すぎます。 テーブルまたはグリッドに「プロジェクト名」と「現在のマイルストーン」を表示するだけの方法はありますか？

**回答**

はい。現在作業中のマイルストーン タスクと、それに関連付けられているタスクを表示するタスク報告書を作成できます。 テーブルまたはリストレポートで実行できます。

**質問**

プルーフの情報をレポートのプロジェクト情報と組み合わせることはできますか？

**回答**

プルーフ承認レポートを作成した場合は、テキストモードを使用して、プロジェクト情報を列に取り込むことができます。 例えば、列内のプロジェクト名を参照する場合は、次を使用します。

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

**質問**

また、プロジェクトに関連するプルーフデータのレポートに関する詳細も知りたいです。 例えば、プルーフの決定とコメントを含むプロジェクトレポートなどです。

**回答**

プロジェクト情報とプルーフ情報を 1 つのレポートで参照するには、プルーフ承認レポートを作成する必要があります。 現在、プルーフからのコメントはこのレポートに取り込むことができませんが、プルーフの各承認者の決定は、独自の行項目の「承認者の決定」列の下にあります。

**質問**

単一ページのステータス（多くの列）を作成するために、sharecol を頻繁に使用します。 ただし、レポートを作成した後にページの上部に列を追加しようとすると、戻って変更するのにかなりの時間がかかります。 このような変更を行うためのヒントやコツはありますか？

**回答**

テキストモードの列リストの上部に列を配置する場合は、手動で列の番号を変更する必要があります。

ただし、最初の列が共有列になっているレポートを既に作成していて、別の共有列をリストの上部に配置する場合は、この方が簡単です。

レポートエディターで、新しい列をいくつか追加し、列（表示）画面の左端にドラッグします。 これを行った後、左側の列が何であったかを見ると、テキストモードの列番号がすべて増分されていることがわかります。 空白の列を必要な数だけドラッグします。 必ず空白の列に何かを入れてから保存してください。そうしないと、削除されます。

**質問**

複数のプロジェクトにバグが発生している場合、最終的なバグレポートに関して、複数のプロジェクトに対してレポートを行う方法を教えてく？？さい。

**回答**

作業をどのように整理したかに応じて、ポートフォリオまたはプロジェクトでフィルタリングできます。

リクエストキューでフィルタリングすることもできます。 プロジェクトごとにリクエストキューを設定できます。このキューで、顧客ユーザーをレビュー担当者として作成し、共有したリクエストキューに直接ログインしてチケットを送信できます。

**質問**

最初のレポートはプロジェクト名やプロジェクト名に基づいていましたが、タスクについても実行できます。できる場合は、タスク名が頻繁に異なる可能性があるので、タスクをグループ化する最適な方法はどうでしょうか…ありがとうございました！

**回答**

これらのすべてのレポートは、トラッキング方法に応じて、タスクレポート、イシューレポートまたはプロジェクトレポートのいずれかとして実行できます。

タスクをグループ化する一般的な方法は、まずプロジェクト名でグループ化し、次に各プロジェクト内のタスク名でグループ化することです。 このようにして、同じ名前のタスクが 2 つある場合、どのプロジェクトにあるかを簡単に確認できます。

**質問**

どのプルーフが傑出しているか、どのタスクとプロジェクトに結び付けられているか、いつルーティングされたか、いつ期限か、誰がモデレーターと承認者かを知りたいと思います。

**回答**

未完了のプルーフは、プルーフ承認レポート内で、決定を待機/次に等しい/True を選択することでフィルタリングできます。 まだ決定を行っていない人に知らせる承認者の列があります。

テキストモードを使用して、プルーフが関連付けられているタスクまたはプロジェクトを参照できます（以下の例を参照）。

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name
valueformat=HTML
```

ルーティング日、期限、モデレーターに関しては、これらのフィールドは現在、Workfrontのレポートに取り込めないため、プルーフを直接クリックして表示する必要があります。

**質問**

リクエストの完了後に依頼者に自動的に送信するカスタムフォームを設定できますか？ 「顧客満足度」調査と似ていますか？

**回答**

ニーズに合わせて実行できる操作を 1 つ示します。 実際の完了日が入力された後、「入力者」にメールを送信するイシューにリマインダー通知を添付できます。 入力者は、問題を作成したユーザーです。

「アクションレビュー後（AAR）に入力するリマインダー」に対してウェビナーで行ったのと同様にリマインダー通知を作成しますが、これが問題のリマインダーになる場合を除きます。 調査用のメールテンプレートを作成し、調査へのリンクを提供する必要がある場合もあります。 リマインダー通知は、各問題に手動で適用する（または一括編集を使用する）必要があります。

手動の手順を自動化できるので統合の方が良いのですが、リマインダー通知はすぐに行えます。

**質問**

テンプレートタイプ別にプロジェクトを示すレポートを作成しました。 プロジェクト所有者の一覧を表示できますが、プロジェクトに割り当てられたユーザーの一覧を表示することはできません。

**回答**

プロジェクトチーム（「スタッフ」タブ）をプロジェクトレポート内の列に取り込む場合は、テキストモードで作成する必要があります。 テキストモードは次のとおりです。

```
displayname=Staffing 
listdelimiter=<p> 
listmethod=nested(projectUsers).lists 
textmode=true
type=iterate 
valuefield=user:name 
valueformat=HTML
```

## AAR エンゲージメントレポートのテキストモードコード

```
column.0.displayname=Task Details
column.0.value=<b>Project Name:</b>&nbsp;
column.0.valueformat=HTML
column.0.sharecol=true
column.1.valuefield=project:name
column.1.valueformat=HTML
column.1.sharecol=true
column.2.value=<br>
column.2.valueformat=HTML
column.2.sharecol=true
column.3.value=<b>Task Name:</b>&nbsp;
column.3.valueformat=HTML
column.3.sharecol=true
column.4.valuefield=name
column.4.valueformat=HTML
column.4.sharecol=true
column.5.value=<br>
column.5.valueformat=HTML
column.5.sharecol=true
column.6.value=<b>Task Owner:</b>&nbsp;
column.6.valueformat=HTML
column.6.sharecol=true
column.7.valuefield=assignedTo:name
column.7.valueformat=HTML
column.7.sharecol=true
column.8.value=<br>
column.8.valueformat=HTML
column.8.sharecol=true
column.9.value=<b>Actual Completion Date:</b>&nbsp;
column.9.valueformat=HTML
column.9.sharecol=true
column.10.valuefield=actualCompletionDate
column.10.valueformat=HTML
column.11.displayname=Name of Reviewer
column.11.linkedname=Name of Reviewer
column.11.namekey=view.relatedcolumn
column.11.namekeyargkey.0=Name of Reviewer
column.11.namekeyargkey.1=name
column.11.querysort=DE:Name of Reviewer:name
column.11.valuefield=Name of Reviewer:name
column.11.valueformat=customReferenceObjectAsString
column.12.displayname=AAR 1
column.12.description=In your view, does the work match stakeholders’ expectations? Did we achieve the intended results?
column.12.value=<b>AAR 1 Score:</b>&nbsp;
column.12.valueformat=HTML
column.12.sharecol=true
column.13.valuefield=AAR 1 - In your view, does the work match stakeholders’ expectations? Did we achieve the intended results?
column.13.valueformat=customDataLabelsAsString
column.13.sharecol=true
column.14.value=<br>
column.14.valueformat=HTML
column.14.sharecol=true
column.15.value=<br><b>AAR 1 User Comment:</b>&nbsp;
column.15.valueformat=HTML
column.15.sharecol=true
column.16.valuefield=AAR 1 User Comment
column.16.valueformat=customDataLabelsAsString
column.17.linkedname=direct
column.17.namekey=AAR 1 Reviewer Comment
column.17.querysort=DE:AAR 1 Reviewer Comment
column.17.valuefield=AAR 1 Reviewer Comment
column.17.valueformat=customDataLabelsAsString
column.18.linkedname=direct
column.18.displayname=AAR 1 Needs Attn
column.18.querysort=DE:AAR 1 Needs Attention
column.18.valuefield=AAR 1 Needs Attention
column.18.valueformat=customDataLabelsAsString
column.19.linkedname=direct
column.19.displayname=AAR 1 Needs Attn Notes
column.19.querysort=DE:AAR 1 Needs Attention Notes
column.19.valuefield=AAR 1 Needs Attention Notes
column.19.valueformat=customDataLabelsAsString
column.20.displayname=AAR 2
column.20.description=Do You Believe This Work Will Make an Impact?
column.20.value=<b>AAR 2 Score:</b>&nbsp;
column.20.valueformat=HTML
column.20.sharecol=true
column.21.valuefield=AAR 2 - Do You Believe This Work Will Make an Impact?
column.21.valueformat=customDataLabelsAsString
column.21.sharecol=true
column.22.value=<br>
column.22.valueformat=HTML
column.22.sharecol=true
column.23.value=<br><b>AAR 2 User Comment:</b>&nbsp;
column.23.valueformat=HTML
column.23.sharecol=true
column.24.valuefield=AAR 2 User Comment
column.24.valueformat=customDataLabelsAsString
column.25.linkedname=direct
column.25.namekey=AAR 2 Reviewer Comment
column.25.querysort=DE:AAR 2 Reviewer Comment
column.25.valuefield=AAR 2 Reviewer Comment
column.25.valueformat=customDataLabelsAsString
column.26.linkedname=direct
column.26.displayname=AAR 2 Needs Attn
column.26.querysort=DE:AAR 2 Needs Attention
column.26.valuefield=AAR 2 Needs Attention
column.26.valueformat=customDataLabelsAsString
column.27.linkedname=direct
column.27.displayname=AAR 2 Needs Attn Notes
column.27.querysort=DE:AAR 2 Needs Attention Notes
column.27.valuefield=AAR 2 Needs Attention Notes
column.27.valueformat=customDataLabelsAsString
column.28.displayname=AAR 3
column.28.description=Are you proud of the work you did on this?
column.28.value=<b>AAR 3 Score:</b>&nbsp;
column.28.valueformat=HTML
column.28.sharecol=true
column.29.valuefield=AAR 3 - Are you proud of the work you did on this?
column.29.valueformat=customDataLabelsAsString
column.29.sharecol=true
column.30.value=<br>
column.30.valueformat=HTML
column.30.sharecol=true
column.31.value=<br><b>AAR 3 User Comment:</b>&nbsp;
column.31.valueformat=HTML
column.31.sharecol=true
column.32.valuefield=AAR 3 User Comment
column.32.valueformat=customDataLabelsAsString
column.33.linkedname=direct
column.33.namekey=AAR 3 Reviewer Comment
column.33.querysort=DE:AAR 3 Reviewer Comment
column.33.valuefield=AAR 3 Reviewer Comment
column.33.valueformat=customDataLabelsAsString
column.34.linkedname=direct
column.34.displayname=AAR 3 Needs Attn
column.34.querysort=DE:AAR 3 Needs Attention
column.34.valuefield=AAR 3 Needs Attention
column.34.valueformat=customDataLabelsAsString
column.35.linkedname=direct
column.35.displayname=AAR 3 Needs Attn Notes
column.35.querysort=DE:AAR 3 Needs Attention Notes
column.35.valuefield=AAR 3 Needs Attention Notes
column.35.valueformat=customDataLabelsAsString
column.36.displayname=Done
column.36.valuefield=Review Complete
column.36.valueformat=customDataLabelsAsString
```
