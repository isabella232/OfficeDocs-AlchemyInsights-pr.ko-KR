---
title: 암호 동기화 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664932"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="c04dc-102">암호 동기화 문제 해결</span><span class="sxs-lookup"><span data-stu-id="c04dc-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="c04dc-103">암호 동기화 문제를 해결 하려면이 AAD 연결 문제 해결 작업을 사용 하 여 암호가 동기화 되지 않는 이유를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="c04dc-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="c04dc-104">시작 하려면 [직접 동기화 관리](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="c04dc-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="c04dc-105">Azure AD Connect 서버에서 새 Windows PowerShell 세션을 열고 **관리자 권한으로 실행** 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c04dc-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="c04dc-106">ExecutionPolicy RemoteSigned 또는 ExecutionPolicy 제한이 없는 경우 실행 합니다.</span><span class="sxs-lookup"><span data-stu-id="c04dc-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="c04dc-107">Azure AD Connect 마법사를 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="c04dc-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="c04dc-108">다음에 대 한 **문제 해결**> 추가 작업 페이지로 이동  >  **Next**합니다.</span><span class="sxs-lookup"><span data-stu-id="c04dc-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="c04dc-109">**시작** 을 선택 하 여 PowerShell 문제 해결 메뉴를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="c04dc-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="c04dc-110">**암호 동기화 문제 해결**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c04dc-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="c04dc-111">이 문제는 일반적으로 특정 사용자 계정에 대해 암호가 동기화 되지 않은 경우에 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="c04dc-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="c04dc-112">**참고 사항** 마지막으로 성공한 암호 동기화가 잠시 전에 암호 동기화가 실패 합니다.</span><span class="sxs-lookup"><span data-stu-id="c04dc-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="c04dc-113">암호 동기화 문제 해결에 대 한 자세한 내용은 [AZURE AD Connect sync를 통한 암호 해시 동기화 문제 해결](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="c04dc-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>