---
title: エキスパートに質問 – 品質とエンゲージメントを測定
description: 品質とエンゲージメントに関する疑問に答えるレポートの作成方法を学びましょう。 このウェビナーは2019年11月13日に録画されました。
feature: Reports and Dashboards
topic: Administration, Integrations
doc-type: feature video
team: Technical Marketing
kt: 9914
exl-id: 76a8e418-71c7-414a-9938-e64e4e73c184
duration: 3980
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '1217'
ht-degree: 0%

---

# エキスパートに質問 – 品質とエンゲージメントを測定

品質とエンゲージメントに関する疑問に答えるレポートの作成方法を学びましょう。 このウェビナーは2019年11月13日に録画されました。

>[!VIDEO](https://video.tv.adobe.com/v/341120/?quality=12)

## Q&amp;A

**質問**

フィルターを使用できるフィールドもありますが、フィルターでグループ化しようとすると使用できないフィールドもあります。 一貫性のあるオプションを提供していますか？

**回答**

レポートツールでは、動的なフィールドや、チェックボックスフィールドなど、一度に複数の選択を選択できるフィールドでグループ化することはできません。 選択肢が多い場合でも、1つの値を持つフィールドでのみグループ化できます。

チェックボックスで絞り込んで表示することもできますが、グループ化することはできません。

**質問**

担当業務のイテレーションの例では、プライマリを太字で表示できますか？

**回答**

イテレーションでは、主要な担当業務を特定できます。 これはvalueexpressionで行う必要がありますが、HTML コードはvalueexpressionで認識されません。 そのため、その役割を主要なものとして特定する別の方法を考え出す必要があります。 このコードでは、プライマリロール名の前後に「**」を付けます。 試してみて、好きなように見てください：

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

Designerがこのユーザーの主要な役割です。

**質問**

こんにちは！ 私は、エディトリアルチームのために、記事がライフサイクルのどの段階にあるのかを追跡するワークフローを作成しています（最初の執筆/部署のレビュー/最終編集/公開）。 現在どのマイルストーンやタスクにあるのかを簡単に確認したい場合。 私が受けているフィードバックは、標準的なマイルストーンビュー（赤または緑のシェーディング付き）が「ビジーで複雑」すぎることです。 「プロジェクト名」と「現在のマイルストーン」を表またはグリッドに表示する方法はありますか？

**回答**

はい。 現在作業しているマイルストーンタスクと、そのタスクに関連するタスクを表示するタスクレポートを作成できます。 これは、テーブルまたはリストレポートで実行できます。

**質問**

レポートにプルーフ情報とプロジェクト情報を組み合わせることはできますか？

**回答**

プルーフ承認レポートを作成した場合、テキストモードを使用してプロジェクト情報を列に取り込むことができます。 例えば、列内のプロジェクト名を参照する場合は、次のコマンドを使用できます。

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

**質問**

プロジェクトに関連するプルーフデータに関するレポートの詳細も知りたい。 例えば、プルーフの決定とコメントを含むプロジェクトレポートがあります。

**回答**

1つのレポートでプロジェクト情報とプルーフ情報を参照するには、プルーフ承認レポートを作成する必要があります。 現在、プルーフからのコメントはこのレポートに取り込めませんが、各プルーフ承認者の決定は、「承認者の決定」列の下にある独自の行アイテムにあります。

**質問**

単一ページステータス（多くの列）を作成するために、よくsharecolを使用します。 しかし、レポートを作成した後、ページの上部に列を追加すると、戻って修正するのに非常に時間がかかります。 このような変化を起こすためのヒントやコツはありますか？

**回答**

テキストモードの列リストの上部に列を配置する場合は、列の番号を手動で変更する必要があります。

しかし、最初の列が共有列であるレポートを既に作成しており、リストの上部に別の共有列を配置したい場合は、これは簡単です。

レポートエディターで、新しい列をいくつか追加し、列（表示）画面の左端にドラッグします。 これを行うと、以前の左側の列を見てみると、テキストモードの列番号がすべて増分されていることに気づくでしょう。 必要な数だけ空の列をドラッグします。 保存する前に、必ず空白の列に何かを入れてください。そうしないと、削除されます。

**質問**

こんにちは – 最後のバグレポートに関して – 複数のプロジェクトに対してバグが発生している場合、複数のプロジェクトに対してレポートを実行する方法？?

**回答**

作業方法に応じて、ポートフォリオやプロジェクトで絞り込むことができます。

リクエストキューでフィルタリングすることもできます。 各プロジェクトにリクエストキューを設定して、顧客ユーザーをレビューアーとして作成し、共有したリクエストキューに直接ログインしてチケットを送信できるようにする場合があります。

**質問**

最初のレポートはプロジェクト/プロジェクト名に基づいていました。タスクでも実行できます。タスク名が頻繁に異なる可能性があるため、タスクをグループ化する最善の方法は何ですか？

**回答**

これらのレポートは、タスク、イシュー、プロジェクトレポートのどちらでも、状況の追跡方法に応じて作成できます。

タスクをグループ化する一般的な方法は、最初にプロジェクト名でグループ化し、次に各プロジェクト内のタスク名でグループ化することです。 これにより、同じ名前のタスクが2つ存在する場合、どのプロジェクトに属しているかを容易に把握できます。

**質問**

どのプルーフが優れているか、どのようなタスクやプロジェクトに関連付けられているか、いつルーティングされたか、いつ納期が来るか、誰がモデレーターで承認者なのかを知りたいと思います。

**回答**

未処理のプルーフは、プルーフ承認レポート内で決定待ち/等価/Trueでフィルタリングできます。 「承認者」の列があり、まだ決定を下していない人が表示されます。

テキストモードを使用して、プルーフが関連付けられているタスクやプロジェクトを参照できます（以下の例を参照）。

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

ルーティング日、期日、モデレーターについては、現在、これらのフィールドはWorkfrontのレポートに表示できないため、プルーフを直接クリックして確認する必要があります。

**質問**

リクエストが完了したら、依頼者に自動的に送信するカスタムフォームを設定できますか？ 「顧客満足度」調査のようなものを選びましょう？

**回答**

そこで、次のことが可能になります。 実際の完了日が入力された後に「入力者」に電子メールを送信する問題にリマインダー通知を添付できます。 「入力者」は、イシューを作成した人物です。

「After Action Review （AAR）」のウェビナーと同様にリマインダー通知を作成しますが、これは問題リマインダーになります。 アンケートへのリンクを提供するために、メールテンプレートを作成することもできます。 各問題にリマインダー通知を手動で適用する必要があります（または一括編集を使用する）。

手作業によるステップを自動化できるため、統合の方が優れていますが、リマインダー通知はすぐに実行できます。

**質問**

テンプレートタイプ別のプロジェクトを示すレポートを作成しました。 プロジェクトに割り当てられたメンバーではなく、プロジェクトオーナーをリストアップできます。

**回答**

プロジェクトチーム（人員配置タブ）をプロジェクトレポート内の列に取り込む場合は、テキストモードでこれを作成する必要があります。 テキストモードは次のとおりです。

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
