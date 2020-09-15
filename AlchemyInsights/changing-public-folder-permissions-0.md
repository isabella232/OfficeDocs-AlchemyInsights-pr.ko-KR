---
title: 공용 폴더 사용 권한 변경
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: a2a902e8fdfd8628772364c173979c633d25a169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714253"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="ff049-102">공용 폴더 사용 권한 변경</span><span class="sxs-lookup"><span data-stu-id="ff049-102">Changing public folder permissions</span></span>

<span data-ttu-id="ff049-103">공용 폴더 사용 권한은 Outlook의 사용자 및 관리자가 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff049-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="ff049-104">관리자는 다음을 수행 하 여 EAC (Exchange 관리 센터)에서 사용 권한을 제어할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff049-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="ff049-105">Microsoft 365 관리 센터에서 **관리 센터** \> **Exchange**로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="ff049-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="ff049-106">**공용 폴더**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="ff049-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="ff049-107">여기에서 보안 그룹을 사용 권한에 할당 하 여 개별 공용 폴더에 대 한 사용 권한을 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff049-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="ff049-108">최종 사용자가 공용 폴더 권한을 변경 하려면 사용자에 게 해당 폴더에 대 한 소유자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ff049-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

<span data-ttu-id="ff049-109">공용 폴더 사용 권한 문제를 해결 하기 위해 [public folder 권한 문제를 진단 하 고 해결 하는 방법](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) 에 설명 된 절차를 따르세요.</span><span class="sxs-lookup"><span data-stu-id="ff049-109">Please follow the procedure described in [How to diagnose and fix public folder permission issues](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) to troubleshoot public folder permission issues.</span></span>

<span data-ttu-id="ff049-110">**참고**: 공용 폴더에 대 한 사용 권한을 변경 하려고 할 때 발생할 수 있는 알려진 문제가 몇 가지 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff049-110">**Note**: There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="ff049-111">자세한 내용은 다음 문서를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="ff049-111">See the following articles for more information.</span></span>

- [<span data-ttu-id="ff049-112">EAC의 공용 폴더 하위 폴더에 사용 권한을 적용할 수 없음</span><span class="sxs-lookup"><span data-stu-id="ff049-112">Can't apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [<span data-ttu-id="ff049-113">공용 폴더에 액세스할 때 "로컬 포리스트에서 사서함을 찾을 수 없습니다." 오류</span><span class="sxs-lookup"><span data-stu-id="ff049-113">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
