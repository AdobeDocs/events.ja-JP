---
title: 微調整された AI モデルを使用して、Marketo Engageのデータ分類を改善する
description: Marketo Engageで微調整された AI モデルを使用して、スパムを検出する方法、役職をペルソナに一致させる方法、Webhook を使用して開いているテキストフィールドを分類する方法について説明します。
topic: Artificial Intelligence
role: User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 0
last-substantial-update: 2025-08-29T00:00:00Z
jira: KT-18864
source-git-commit: b8f3c336420c4c56561539183e7542d9830eb1af
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---


# 微調整された AI モデルを使用して、Marketo Engageのデータ分類を改善する

売上高の運用担当者は、スパムフォームの送信、ペルソナを決定するための役職でのキーワードのマッチング、データからインサイトを抽出するのが難しい雑然としたオープンテキストフィールドなどに苦労している可能性があります。 これらのデータ分類の課題により、セグメント化、パーソナライゼーションおよびレポートが妨げられ、チームがデータを活用できず、カスタマイズされたコンテンツをオーディエンスに送信するのが困難になります。

大規模な言語モデル（LLM）の微調整が、これらの永続的なデータ問題にどのように役立つかについて説明します。 カスタムトレーニング済みモデルが、スパムフィルタリングの精度を大幅に高め、ペルソナ分類を自動化し、非構造化された入力をインテリジェントに分類し、AI をMarketo Engageに取り込む方法について説明します。

以下について説明します。

* AI によってMarketo Engageのデータ分類が大幅に向上する実際のユースケース。
* 独自のデータを使用して LLM を微調整する方法（例として OpenAI を使用）。
* Webhook を介してMarketo Engageの微調整モデルを使用。

>[!VIDEO](https://video.tv.adobe.com/v/3471388/?learn=on&enablevpops)

## データ分類のための AI のユースケース

* **スパム検出** AI モデルは CAPTCHA よりもパフォーマンスが高く、誤検知や誤検知を減らし、セールスチームの時間を節約します。
* **ペルソナマッチング** AI は、役職名（スペルミスやその他の言語の場合でも）をペルソナに正確にマッピングし、リードスコアリングとセグメント化を改善します。
* **オープンテキストフィールドの分類** AI は、様々なアトリビューションソースをグループ化し、スペルミスや言語の処理を行い、より豊富なインサイトとレポートを可能にします。
* **カスタマイズ** 微調整されたモデルにより、カテゴリごとにルールと説明を定義して、結果を完全に制御できます。


## その他のリソース

* [Marketo Engage向けの微調整された AI モデル ](https://nation.marketo.com/t5/champion-program-blogs/fine-tuned-ai-models-for-marketo/ba-p/357019)
* [Webhook クイックスタートガイド ](https://nation.marketo.com/t5/champion-program-blogs/webhook-quick-start-guide/ba-p/345717#M2640)
* [ChatGPT とMarketo Engageの統合 ](https://nation.marketo.com/t5/champion-program-blogs/integrating-chatgpt-with-marketo/ba-p/346886)
* [ セルフサービスフロー手順ガイド ](https://nation.marketo.com/t5/champion-program-blogs/self-service-flow-steps-guide/ba-p/357008)