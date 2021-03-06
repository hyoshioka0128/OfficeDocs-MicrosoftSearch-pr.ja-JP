---
title: FAQ
ms.author: anfowler
author: adefowler
manager: shohara
ms.audience: Admin
ms.topic: reference
ms.service: mssearch
localization_priority: Normal
search.appverid:
- BFB160
- MET150
- MOE150
description: エンタープライズ検索と Microsoft Search についてよく寄せられる質問に対する回答です
ms.openlocfilehash: edfb8346263d60184d8655afa24118ed4b3e3bca
ms.sourcegitcommit: 68087149c769a7cdde80944dd9c9933d2bf4a23f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/18/2019
ms.locfileid: "38699795"
---
# <a name="frequently-asked-questions"></a>よく寄せられる質問

以下は、よく寄せられる質問の一覧です。

> [!TIP]
> ここで質問に対する回答が得られなかった場合は、 この記事のフィードバックを使用してご質問ください。

## <a name="is-advanced-query-understanding-supported"></a>高度なクエリ理解はサポートされていますか?

はい、大規模な語句からクエリの目的を解析します。この機能は、AI を使用して、検索の目的に影響を与えないクエリにユーザーが追加する一般的な不必要な語句を調べます。たとえば、ユーザーが自分のパスワードを*変更する方法について詳しく説明して*いる場合は、「 *change password*」のような関連する用語に基づいて、クエリとトリガーから重要度の低い単語を抽出します。
  
この機能は、Microsoft 365[管理センター](https://admin.microsoft.com)で設定されたキーワードより優先されません。
  
## <a name="can-you-search-for-files-on-premises"></a>オンプレミスのファイルを検索できますか?

はい。 SharePoint のハイブリッド展開がある場合は、オンプレミスの[sharepoint](http://sharepoint.com/)ファイルを検索できます。
  
## <a name="how-do-i-make-bing-the-default-search-engine-for-people-in-my-org"></a>自分の組織のユーザーに対して Bing を既定の検索エンジンとして設定する方法を教えてください。

次の手順では、既定の検索エンジン、既定のホームページ、および既定のブラウザーを設定して、 [Bing](https://Bing.com)で Microsoft search の最適な環境をユーザーに提供します。

- [Microsoft Edge を既定のブラウザーとして設定する](set-default-browser.md)
- [Bing を既定の検索エンジンとして設定する](set-default-search-engine.md)
- [Bing.com をエンタープライズ ホームページとして設定する](set-default-homepage.md)

  
## <a name="how-are-my-search-results-protected"></a>検索結果に対する保護について教えてください。

信頼されたクラウドからの結果にアクセスするには、 [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/)認証が必要です。 認証されたユーザーには、そのユーザーがアクセス権を持つコンテンツのみが表示されます。 検索クエリは識別されないため、ログはパブリック[Bing](https://Bing.com)検索トラフィックから分離されます。 このレベルの保護が提供されているのは、業界内でも Microsoft Search だけです。

## <a name="can-i-search-across-federated-organizations"></a>フェデレーション組織間を検索できますか?

いいえ。

## <a name="where-can-i-get-info-about-office-365-and-microsoft-365-compliance-tiers-and-categories"></a>Office 365 および Microsoft 365 のコンプライアンス階層とカテゴリに関する情報はどこで入手できますか?

「[業界標準と規制に関するコンプライアンス フレームワーク](https://download.microsoft.com/download/B/2/7/B27B3EF3-8849-4C18-8BA4-5AD755728620/Compliance%20Framework_customer%20guidance.pdf)」(PDF ダウンロード) で詳細を入手できます。

## <a name="can-users-earn-microsoft-rewards-points-with-their-work-or-school-account"></a>ユーザーは職場または学校のアカウントで Microsoft リワード ポイントを獲得できますか?

Microsoft Search では、エンタープライズ ユーザーが職場または学校のアカウントでサインインする必要があります。 ただし、ユーザーはこれらのアカウントで Microsoft リワード プログラムに参加またはサインインすることはできません。 しかし、エンタープライズ ユーザーにリワード ポイントが発生する場合があります。 これは、Microsoft Search ユーザーが <a href="https://www.microsoft.com/welcome?rtc=1">Microsoft アカウント</a>で作成されたリワード アカウントを持っている場合に発生する可能性があります。 (Microsoft アカウントに関連付けられている電子メール アドレスに、Outlook.com、Hotmail.com、Gmail、Yahoo、またはその他のプロバイダーからのものが使用できます。) ユーザーが同じブラウザー セッションで仕事用アカウントと Microsoft アカウントの両方で交互にサインインする場合、リワード アカウントにポイントが加算される場合があります。 ユーザーは、Cookie をクリアすることにより、Microsoft Search での検索中にポイントの発生を停止できます。 

