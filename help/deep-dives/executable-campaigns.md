---
title: 実行可能なキャンペーン — 実行可能ファイルが効率と影響をどのように促すかを説明します。
description: このセッションは、Marketoの管理者やキャンペーン運用の専門家向けにカスタマイズされ、実行可能なキャンペーンの理解とデプロイに焦点を当てて、キャンペーンとプログラムに価値を与え、効率性を高め、成長を促進します。
role: Developer, User
level: Intermediate, Experienced
doc-type: Event
duration: 3778
last-substantial-update: 2024-03-07T00:00:00Z
jira: KT-15098
thumbnail: 3427704.jpeg
exl-id: cfea1a1a-2d29-4cf6-b633-aa2a2523114e
source-git-commit: 5edfadf5b805161f9624068f70a7b4830ab84d72
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# 実行可能なキャンペーン — 実行可能ファイルが効率と影響をどのように高めるかを説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3427704/?learn=on)

**モデレート実行者** クリス・ウィリス
**スピーカー** Courtny Edwards-Jones と Jane Musatova

## 概要

Adobeチャンピオンディープダイブのこのエディションでは、Marketoでの実行可能なキャンペーンの使用方法と、それらを使用してプロセスを合理化し、データの正確性を確保する方法の例を示します。 実行可能キャンペーンは、同期的にフローを実行するスマートキャンペーンの一種で、異なるステップ間の依存関係を確保します。 これらを使用して、次の手順に進む前に、データの標準化やリードの選定など、失敗したプロセスを自動的に再試行することができます。 このドキュメントでは、親キャンペーンとネストされた実行可能ファイルの使用、および Web フックや待機ステップを使用できないなど、実行可能なキャンペーンの制限についても説明します。

## 実行可能なキャンペーンを使用する目的は何ですか？

実行可能なキャンペーンを使用する目的は、Marketoで複雑なワークフローを合理化し、自動化することです。 実行可能なキャンペーンでは、キャンペーンの次の手順に進む前に完了する必要がある一連のアクションを定義できます。 これにより、続行する前に各アクションが完全に実行され、エラーや不完全なプロセスのリスクが軽減されます。 実行可能なキャンペーンを使用して、失敗したプロセスの再試行、データの標準化とエンリッチメント、リードの選定、注目のアクションのキャプチャなどをおこなうことができます。 マーケティングオペレーションをより効率的かつ整理的に管理および自動化する方法を提供します。

## 実行可能なキャンペーンとは何ですか？また、その機能は何ですか？

実行可能なキャンペーンは、Marketoの一種のスマートキャンペーンで、1 つのキャンペーン内で複数のフローを順次実行できます。 これは、各フローが次のフローが開始する前に、確実に完全に実行されるように設計されています。 これは、フローを非同期的に実行し、複数のフローを並行して実行できるリクエストキャンペーンとは異なります。

実行可能なキャンペーンを作成するには、キャンペーンを作成する際に「実行可能ファイル」ボックスをオンにする必要があります。 作成後は、データ値の変更、E メールの送信、プログラムステータスの更新など、フローステップをキャンペーンに追加できます。 ただし、実行可能なキャンペーンにはいくつかの制限があります。 実行可能なキャンペーン内で、トリガー、Web フック、待機ステップを使用することはできません。

実行可能なキャンペーンは、相互に依存関係を持つプロセスで役立ちます。次のプロセスを開始する前に、フローを完了する必要があります。 運用プロセスの合理化、データ処理の合理化、エラーやバックログのリスクの最小化に役立ちます。 実行可能なキャンペーンを使用すると、次のキャンペーンに進む前にプロセスの各手順が完了していることを確認でき、マーケティング操作の効率と正確性が向上します。