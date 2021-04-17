---
title: 소유자는 Outlook을 사용하여 하위 폴더를 만들 수 없습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836141"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="96a7c-102">소유자는 Outlook을 사용하여 하위 폴더를 만들 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="96a7c-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="96a7c-103">**Outlook을 사용하여 하위 폴더를 만들 때 공용 폴더 소유자에게 지속적인 문제가 발생합니다. 문제가 곧 해결될 예정입니다.**</span><span class="sxs-lookup"><span data-stu-id="96a7c-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="96a7c-104">그동안 다음 해결 방법 중 하나를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="96a7c-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="96a7c-105">해당 문제가 데스크톱 Windows용 Outlook(모든 버전)에만 영향을 끼치므로 MAC용 Outlook을 사용하여 하위 폴더를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="96a7c-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="96a7c-106">관리자가 EXO Shell 또는 EAC를 사용하여 하위 폴더를 만들도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="96a7c-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="96a7c-107">사용자의 DefaultPublicFolderMailbox/EffectivePublicFolderMailbox를 문제가 발생하는 폴더의 콘텐츠 사서함이 아닌 다른 사서함으로 변경</span><span class="sxs-lookup"><span data-stu-id="96a7c-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="96a7c-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="96a7c-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="96a7c-109">한 시간 정도 기다린 후 Outlook 클라이언트 다시 시작</span><span class="sxs-lookup"><span data-stu-id="96a7c-109">Wait for an hour, restart outlook client</span></span>