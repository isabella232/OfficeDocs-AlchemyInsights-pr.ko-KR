---
title: 동기화 되지 않는 Active Directory
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697635"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="38cd8-102">동기화 되지 않는 Active Directory</span><span class="sxs-lookup"><span data-stu-id="38cd8-102">Active Directory not syncing</span></span>

<span data-ttu-id="38cd8-103">"최근 동기화 하지 않음"과 같은 동기화 오류가 발생 하거나 Office 관리 포털에서 디렉터리 동기화 상태를 확인 하는 경우, "마지막으로 3 일 넘게 완료 되었습니다." 라는 메시지가 표시 되 면 AADConnect에 잘못 된 설정이 있거나 동기화를 수행 하는 데 사용 권한이 부족 한 것일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38cd8-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="38cd8-104">빠른 설정을 사용 하 여 AADConnect을 다시 설치 하면 문제를 빠르게 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38cd8-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="38cd8-105">[최신 버전의 AADConnect를 다운로드](https://go.microsoft.com/fwlink/?LinkId=615771)합니다.</span><span class="sxs-lookup"><span data-stu-id="38cd8-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="38cd8-106">[빠른 설치에 대 한 지침을 따릅니다](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="38cd8-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="38cd8-107">AADConnect 서비스 계정에 대한 자세한 내용은 [Azure AD Connect:계정 및 사용 권한](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="38cd8-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
