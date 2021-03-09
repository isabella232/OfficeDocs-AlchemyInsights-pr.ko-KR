---
title: 공유 사서함을 만드는 동안 프록시 주소 오류
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568296"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="05824-102">사서함 또는 다른 전자 메일 사용 개체를 만드는 동안 프록시 주소 오류</span><span class="sxs-lookup"><span data-stu-id="05824-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="05824-103">전자 메일 사용이 가능한 개체(사서함, 공유 사서함 등)를 만들려고 하여 "프록시 주소 "SMTP:alias@domain.com"가 이미 사용 중입니다."라는 오류가 표시되면 선택한 전자 메일 주소가 이미 조직의 다른 전자 메일 사용 개체에 의해 이동된 것입니다.</span><span class="sxs-lookup"><span data-stu-id="05824-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="05824-104">이 전자 메일 주소가 있는 사용자, 그룹, 공유 사서함 또는 공용 폴더를 찾아 삭제하거나 전자 메일 주소를 변경해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="05824-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="05824-105">그런 다음 사용 가능한 전자 메일 주소가 있는 새 전자 메일 사용 가능 개체를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="05824-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="05824-106">홈 페이지에서 검색을 사용하여 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="05824-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="05824-107">다음 Exchange Online PowerShell 명령을 사용하여 검색할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="05824-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="05824-108">기존 전자 메일 주소를 삭제하지 않는 경우 만들 새 개체의 새 전자 메일 주소를 선택하십시오.</span><span class="sxs-lookup"><span data-stu-id="05824-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  