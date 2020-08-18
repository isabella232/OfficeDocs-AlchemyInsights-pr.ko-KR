---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786895"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="569ed-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="569ed-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="569ed-103">Sharepoint Online 내에서 PowerShell 또는 스크립트 작업</span><span class="sxs-lookup"><span data-stu-id="569ed-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="569ed-104">자세한 내용을 보려면 아래 링크를 방문 하세요.</span><span class="sxs-lookup"><span data-stu-id="569ed-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="569ed-105">SharePoint Online 관리 셸 시작</span><span class="sxs-lookup"><span data-stu-id="569ed-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="569ed-106">다단계 인증을 사용 하 여 SPO PowerShell에 연결 (MFA)</span><span class="sxs-lookup"><span data-stu-id="569ed-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="569ed-107">[SharePoint의 PnP (패턴 및 관행)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) 에는 SPO에 대 한 복잡 한 관리 작업을 수행할 수 있는 PowerShell 명령 라이브러리가 포함 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="569ed-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="569ed-108">SPO 관리 셸을 사용 하 여 연결 하는 데 문제가 있는 경우 최신 버전으로 업데이트 했는지 확인 하 고 *"import-Module Microsoft. PowerShell"* 을 사용 하 여 [모듈을 다시 가져오십시오](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) .</span><span class="sxs-lookup"><span data-stu-id="569ed-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="569ed-109">클라이언트 쪽 개체 모델 스크립트를 실행 하려는 경우에는 로컬 컴퓨터에 [Sharepoint Online 클라이언트 구성 요소 SDK](https://www.microsoft.com/download/details.aspx?id=42038) 를 설치 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="569ed-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="569ed-110">PowerShell에서 스크립트를 실행 하는 데 문제가 있는 경우에는 PowerShell을 관리자 권한으로 실행 하 고 [실행 정책을](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)변경 하는 것을 고려해 야 합니다.</span><span class="sxs-lookup"><span data-stu-id="569ed-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>