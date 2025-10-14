---
title: Experience Manager as a Cloud Serviceでのコンポーネントスクリプトの開発とデプロイのベストプラクティス
description: このセッションでは、アプリケーションのデプロイメントを予測可能にするためにAdobe Experience Managerの開発者が従うことのできる、最新のベストプラクティスについて説明します。 2019 年に Apache Sling 機能として導入され、2020 年以降 AEMaaCS で使用されている事前コンパイル済みバンドルスクリプトは、Adobe Experience Manager コンポーネントの従来のデプロイ方法と比べて、開発者に 2 つの大きな改善点を提供します – 1. スクリプトは、バージョンを管理し、Java API 2 と同様に、明示的な依存関係チェーンを持つことができます。 スクリプトのコンパイルはアプリケーションのビルドプロセス中に実行できるようになり、依存関係の欠落や API の誤った使用など、潜在的なエラーをすばやく見つけることができます ここでは、開発者がプロジェクトを設定して、スクリプトを事前コンパイル済みバンドルとして提供する方法と、ローカルのAdobe Experience Manager Sling Feature Analyzer を使用して API 要件が満たされていることを確認する方法に重点を置き、潜在的なエラーを早期に発見できるようにします。
solution: Experience Manager
feature: Developer Tools
topic: Development
role: Developer, Architect
level: Beginner, Intermediate, Experienced
version: Experience Manager as a Cloud Service
kt: 9177
type: Event
exl-id: 71fa0d10-cea5-416e-a6e5-2c729c7793a6
duration: 1899
source-git-commit: 5c946ab73e78d4243ca310032a10bb8e82228c3d
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 4%

---

# Experience Manager as a Cloud Serviceでのコンポーネントスクリプトの開発とデプロイのベストプラクティス

このセッションでは、アプリケーションのデプロイメントを予測可能にするためにAdobe Experience Managerの開発者が従うことのできる、最新のベストプラクティスについて説明します。 2019 年に Apache Sling 機能として導入され、2020 年以降 AEMaaCS で使用されている事前コンパイル済みバンドルスクリプトは、Adobe Experience Manager コンポーネントの従来のデプロイ方法に比べて、開発者に 2 つの大きな改善点を提供します。1. スクリプトは、バージョンを管理し、Java API 2 と同様に、明示的な依存関係チェーンを持つことができます。 スクリプトのコンパイルはアプリケーションのビルドプロセス中に実行できるようになり、依存関係の欠落や API の誤った使用など、潜在的なエラーをすばやく見つけることができます ここでは、開発者がプロジェクトを設定して、スクリプトを事前コンパイル済みバンドルとして提供する方法と、ローカルのAdobe Experience Manager Sling Feature Analyzer を使用して API 要件が満たされていることを確認する方法に重点を置き、潜在的なエラーを早期に発見できるようにします。

**[Experience League Communities](https://adobe.ly/3zJrS0f)** で会話を続けます。

>[!VIDEO](https://video.tv.adobe.com/v/337851/?quality=12&learn=on&hidetitle=true)

## その他のリソース

- [Adobe Experience Platform ドキュメント &#x200B;](https://experienceleague.adobe.com/docs/experience-platform.html?lang=ja)
- [Adobe Experience Platform 概要](https://experienceleague.adobe.com/docs/experience-platform/landing/home.html?lang=ja)
- [Adobe Experience Platform チュートリアル](https://experienceleague.adobe.com/docs/platform-learn/tutorials/overview.html?lang=ja)
