---
title: 場所の一括作成
ms.author: dawholl
author: dawholl
manager: kellis
ms.date: 12/18/2018
ms.audience: Admin
ms.topic: article
ms.service: mssearch
localization_priority: Normal
search.appverid:
- BFB160
- MET150
- MOE150
ms.assetid: 15c9fada-f7a6-4210-aa6b-028b32217830
ROBOTS: NoIndex
description: Microsoft Search 管理ポータルのインポートツールを使用して、多くの場所を一度に追加する
ms.openlocfilehash: e01c3774439a931dc81f850d8cbee76cc6128a53
ms.sourcegitcommit: 6b531b2ce7253c16251c7089795dedf1d2f3fc33
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/13/2019
ms.locfileid: "38311769"
---
# <a name="bulk-create-locations"></a>場所の一括作成

> [!IMPORTANT]
> この記事は、Bing 管理ポータルの Microsoft Search に適用されます。 ポータルを Microsoft 365 管理センターに移動していますので、後で Bing ポータルの Microsoft Search は削除されます。 Microsoft 365 管理センターを使用して作業を開始することをお勧めします。 [Microsoft Search の概要](overview-microsoft-search.md)。
    
.Csv テンプレートをダウンロードして使用し、場所を一括で作成、編集、および保存します。 
  
1. [場所] セクションの右上隅にある [**インポート**] をクリックします。
    
2. [**ダウンロード場所テンプレート (.csv)] を**クリックする
    
3. .csv ファイルを保存して開きます
    
4. 場所のコンテンツを追加してファイルを保存する

    この .csv ファイルは、CSV UTF-8 ファイルとして保存する必要があります。その他のファイルの種類やエンコーディングでは、インポート エラーが発生する可能性があります
    
5. [場所] セクションの右上隅にある [**インポート**] をクリックします。
    
6. [場所のインポート] ウィンドウで、[**参照**] をクリックし、インポートする .csv ファイルに移動します。 
    
7. **[インポート]** をクリックします

[インポート] および [エクスポート場所] テンプレートのフィールドは同じです。 編集をエクスポート、一括編集、およびインポートするか、空のテンプレートで開始して新しい場所を一括作成することができます。 既存の場所を一括編集するには、管理ポータルからそれらをエクスポートし、必要な編集を行ってからインポートします。

## <a name="prevent-import-errors"></a>インポート エラーを回避する  
必要なデータが存在しないか無効な場合は、エラーが発生します。 エラーによっては、修正の必要がある行や列に関する詳細情報が記載されたログ ファイルが生成される場合があります。 必要な編集を行い、ファイルのインポートを再度実行してください。
  
> [!NOTE]
> すべてのエラーが解決されるまで、場所を作成または編集することはできません。 

エラーが発生しないように、インポート ファイルが正しく書式設定されていることに加えて、次の事項を確認してください。
- インポート テンプレートに存在していたヘッダー行が含まれていること
- インポート テンプレートに存在していたすべての列が含まれていること
- 列の順序がインポート テンプレートと同じであること
- これらの列は空にすることができます。 Id、Last Modified、Last Modified By、および Lat/Long  
このフィールドが空の場合、アドレスに基づいて lat/long を決定します
- 「状態」列は空にできません (この情報は必須です)  
[状態] フィールドに基づいて、場所が下書き、提案済み、スケジュール済み、または自動的に公開されるように保存されます。

また、既存の場所の Id を指定すると、インポートファイルの情報に置き換えられます。

複数の組織を管理するパートナーは、1つの組織からの場所をエクスポートして、別の組織にインポートすることができます。 ただし、インポートする前に Id 列のすべてのデータを削除する必要があります。
  
必須および推奨フィールドの詳細については、「[場所を追加](add-a-location.md)する」を参照してください。

  
