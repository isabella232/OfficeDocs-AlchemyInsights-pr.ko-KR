---
title: Active Directory가 동기화되지 않습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930981"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="5c774-102">Active Directory가 동기화되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5c774-102">Active Directory not syncing</span></span>

<span data-ttu-id="5c774-103">"최근 동기화 없음"처럼 동기화 오류가 수신되거나 Office 관리 포털의 디렉터리 동기화 상태가 "마지막으로 동기화된 지 3일이 지난"이면 AADConnect에 동기화를 수행할 수 있는 권한이 잘못되거나 권한이 부족한 것일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5c774-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="5c774-104">익스프레스 설정을 사용하여 AADConnect를 다시하면 문제가 빠르게 해결될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5c774-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="5c774-105">[최신 버전의 AADConnect를 다운로드합니다.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="5c774-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="5c774-106">[익스프레스 설치에 대한 지침을 따릅니다.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="5c774-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="5c774-107">Azure AD Connect는 Windows Server 2012 이상에 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5c774-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="5c774-108">이 서버는 도메인에 연결되어 있어야 하며 도메인 컨트롤러나 구성원 서버일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5c774-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="5c774-109">Azure AD 요구 사항 및 커넥트 전체 목록은 [Azure AD](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)커넥트.</span><span class="sxs-lookup"><span data-stu-id="5c774-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="5c774-110">AADConnect 서비스 계정에 대한 자세한 내용은 [Azure AD Connect:계정 및 사용 권한](/azure/active-directory/hybrid/reference-connect-accounts-permissions)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="5c774-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
