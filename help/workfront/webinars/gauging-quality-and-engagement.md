---
title: エキスパートへの質問 — 品質とエンゲージメントの評価
description: 品質とエンゲージメントに関する質問に回答するレポートの作成について説明します。 このウェビナーは 2019 年 11 月 13 日に録画されました。
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

# エキスパートへの質問 — 品質とエンゲージメントの評価

品質とエンゲージメントに関する質問に回答するレポートの作成について説明します。 このウェビナーは 2019 年 11 月 13 日に録画されました。

>[!VIDEO](https://video.tv.adobe.com/v/341120/?quality=12)

## Q&amp;A

**質問**

フィルタリングに使用できるフィールドがいくつかありますが、グループ化を試みると使用できません。 一貫性のあるオプションを作成する作業をしているか。

**回答**

レポートツールでは、動的フィールドでグループ化したり、複数の選択肢を一度に選択したりすることはできません（チェックボックスフィールドなど）。 選択肢が多い場合でも、1 つの値を持つフィールドでのみグループ化できます。

チェックボックスでフィルタリングし、表示できますが、グループ化はできません。

**質問**

ジョブロールの反復の例で、プライマリを太字で表示できますか？

**回答**

反復では、主なジョブの役割を特定できます。 これは値式で行う必要がありますが、HTMLコードは値式では認識されません。 そこで、その役割を主なものとして識別する別の方法を考え出す必要があります。 このコードの主な役割名の前後に「**」を付けました。 体験して、好みを確認してください。

```
displayname=All Job Roles 
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("**",{role}.{name},"**"),{role}. {name})
valueformat=HTML
```

これにより、次のようなリストが表示されます。

```
Support Engineer 
QA Engineer 
**Designer**
```

ここで、Designer はこのユーザーの主な役割です。

**質問**

こんにちは！ 私たちの編集チームのためのワークフローを組み立てます。このワークフローでは、記事のライフサイクル内の位置を追跡します（最初の書き込み/部門のレビュー/最終編集/公開）。 現在どのマイルストーンまたはタスクにあるかを簡単に確認したいと考えています。 得られるフィードバックは、標準のマイルストーンビュー（赤または緑の網掛け）ですが、「ビジー状態で複雑です」。 テーブルまたはグリッドに「プロジェクト名」と「現在のマイルストーン」だけを表示する方法はありますか？

**回答**

はい。現在作業中のマイルストーンタスクと、そのタスクに関連付けられているタスクを示すタスクレポートを作成できます。 これは、テーブルまたはリストレポートでおこなうことができます。

**質問**

レポートで、配達確認情報とプロジェクト情報を組み合わせることはできますか？

**回答**

配達確認の承認レポートを作成した場合、プロジェクト情報をテキストモードを使用して列に取り込むことができます。 例えば、列内のプロジェクト名を参照する場合、次のように使用できます。

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

**質問**

また、プロジェクトに関連する配達確認データのレポートに関する詳細を希望します。 例えば、配達確認の決定とコメントを含むプロジェクトレポートなどです。

**回答**

単一のレポートでプロジェクト情報と配達確認情報を参照するには、配達確認の承認レポートを作成する必要があります。 現在、配達確認からのコメントはこのレポートに取り込むことはできませんが、各配達確認の承認者の決定は、「承認者の決定」列の独自の行項目にあります。

**質問**

単一ページのステータス（多数の列）を作成するために、頻繁に sharecol を使用します。 ただし、レポートを作成した後でページの上部に列を追加したい場合は、戻って変更するのに非常に時間がかかります。 このような変更を行うためのヒントやテクニックはありますか？

**回答**

テキストモードの列リストの先頭に列を配置する場合は、列の番号を手動で変更するだけで済みます。

ただし、最初の列が共有列であるレポートを既に作成していて、別の共有列をリストの上に配置すると、作業が容易になります。

レポートエディターで、新しい列を 2 つ追加し、列（表示）画面の左端にドラッグします。 これを行った後、左側の列が何であったかを見てみると、テキストモードの列番号がすべて増加しているのがわかります。 必要な数だけ空白の列をドラッグします。 何かを保存する前に、空白の列に入れてください。入れないと、削除されます。

**質問**

こんにちは — 最終的なバグレポートに関して — 複数のプロジェクトに対してレポートをどのように行うことができますか — 複数のプロジェクトに対してバグが発生している場合??

**回答**

作業内容に応じて、ポートフォリオまたはプロジェクトでフィルタリングできます。

また、リクエストキューに対してフィルターを適用することもできます。 各プロジェクトにリクエストキューを設定し、レビュー担当者として顧客ユーザーを作成して、自分が共有しているリクエストキューに直接チケットをログインして送信できます。

**質問**

最初のレポートはプロジェクト名またはプロジェクト名に基づいていました。これはタスクに対しても実行できます。また、タスク名が異なる場合が多いので、タスク名をグループ化する最善の方法も考えられます。

**回答**

これらのレポートは、追跡方法に応じて、タスク、イシューまたはプロジェクトのレポートとして実行できます。

タスクをグループ化する一般的な方法は、最初にプロジェクト名でグループ化し、次に各プロジェクト内のタスク名でグループ化することです。 同じ名前の 2 つのタスクがある場合は、どのプロジェクトにあるかを簡単に確認できます。

**質問**

未処理の配達確認、関連付けられているタスクとプロジェクト、ルーティングのタイミング、期限、モデレーターと承認者のユーザーを把握したいと考えています。

**回答**

未処理の配達確認は、配達確認の承認レポート内で、決定待ち/次と等しい/True でフィルタリングできます。 承認者の列があり、まだ決定を行っていないユーザーを示します。

テキストモードを使用して、配達確認が関連付けられたタスクまたはプロジェクトを参照できます（以下の例を参照）。

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

ルーティングの日付、期限、モデレーターについては、現在、これらのフィールドをWorkfrontのレポートに取り込むことはできないので、配達確認を直接クリックしてその情報を表示する必要があります。

**質問**

リクエストが完了した後に要求者に自動的に送信するカスタムフォームを設定できますか？ 「顧客満足度」調査のように？

**回答**

必要に応じて実行できることが 1 つあります。 実際の完了日が入力された後、「入力者」に電子メールを送信する問題にリマインダー通知を添付できます。 「入力者」は、イシューを作成したユーザーです。

「Reminder to fill the After Action Review (AAR)」のオンラインセミナで行ったように、リマインダー通知を作成しますが、これは問題のリマインダーです。 調査へのリンクを提供するために、電子メールテンプレートを作成する必要がある場合があります。 各問題にリマインダー通知を手動で適用する（または一括編集を使用する）必要があります。

統合は、手動の手順を自動化できるので、より良い方法ですが、リマインダー通知はすぐにおこなうことができます。

**質問**

テンプレートタイプ別のプロジェクトを示すレポートを作成しました。 プロジェクト所有者のリストは表示できますが、プロジェクトに割り当てられた担当者は表示できません。

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
