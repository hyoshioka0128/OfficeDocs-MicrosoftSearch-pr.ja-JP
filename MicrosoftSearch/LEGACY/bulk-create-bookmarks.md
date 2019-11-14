---
title: ブックマークの一括作成
ms.author: dawholl
author: dawholl
manager: kellis
ms.date: 09/11/2018
ms.audience: Admin
ms.topic: article
ms.service: mssearch
localization_priority: Normal
search.appverid:
- BFB160
- MET150
- MOE150
ms.assetid: def300e7-103c-4e92-a062-28ffa27561d7
ROBOTS: NoIndex
description: Microsoft Search 管理ポータルのインポートツールを使用して、多数のブックマークを一度に作成する
ms.openlocfilehash: 2983a47a8761a2463b25497911024f9bfd069369
ms.sourcegitcommit: 6b531b2ce7253c16251c7089795dedf1d2f3fc33
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/13/2019
ms.locfileid: "38311785"
---
# <a name="bulk-create-bookmarks"></a>ブックマークの一括作成

> [!IMPORTANT]
> この記事は、Bing 管理ポータルの Microsoft Search に適用されます。 ポータルを Microsoft 365 管理センターに移動していますので、後で Bing ポータルの Microsoft Search は削除されます。 Microsoft 365 管理センターを使用して作業を開始することをお勧めします。 [Microsoft Search の概要](overview-microsoft-search.md)。
    
.Csv テンプレートをダウンロードして使用し、ブックマークを一括作成、編集、および保存します。 既存のブックマークを一括編集するには、管理ポータルからそれらをエクスポートし、必要な編集を行ってからインポートします。
  
1. [ブックマーク] セクションの右上隅にある [**インポート**] をクリックします。
    
2. [**ブックマークテンプレートをダウンロードする (.csv)] をクリックします。**
    
3. .csv ファイルを保存して開きます
    
4. ブックマークの内容と設定を追加し、ファイルを保存する

    この .csv ファイルは、CSV UTF-8 ファイルとして保存する必要があります。その他のファイルの種類やエンコーディングでは、インポート エラーが発生する可能性があります
    
5. [ブックマーク] セクションの右上隅にある [**インポート**] をクリックします。
    
6. [ブックマークのインポート] ウィンドウで、[**参照**] をクリックして、インポートする .csv ファイルに移動します。 
    
7. **[インポート]** をクリックします

## <a name="prevent-import-errors"></a>インポート エラーを回避する      
必要なデータが存在しないか無効な場合は、エラーが発生します。 エラーによっては、修正の必要がある行や列に関する詳細情報が記載されたログ ファイルが生成される場合があります。 必要な編集を行い、ファイルのインポートを再度実行してください。

> [!NOTE]
> すべてのエラーが解決されるまで、ブックマークを作成または編集することはできません。 

エラーが発生しないように、インポート ファイルが正しく書式設定されていることに加えて、次の事項を確認してください。
- インポート テンプレートに存在していたヘッダー行が含まれていること
- インポート テンプレートに存在していたすべての列が含まれていること
- 列の順序がインポート テンプレートと同じであること
- 空にできる列は、「Id」、「最終更新日時」、「最終更新者」です
- 「状態」列は空にできません (この情報は必須です)  
状態フィールドに基づいて、ブックマークは、下書き、おすすめ、スケジュール済みとして保存されるか、自動的に公開されます。

また、既存のブックマークの Id を含めると、そのブックマークはインポートファイルの情報に置き換えられます。

複数の組織を管理するパートナーは、1つの組織からブックマークをエクスポートして、別の組織にインポートすることができます。 ただし、インポートする前に Id 列のすべてのデータを削除する必要があります。

必須および推奨フィールドの詳細については、「 [Create bookmarks](create-bookmarks.md)」を参照してください。