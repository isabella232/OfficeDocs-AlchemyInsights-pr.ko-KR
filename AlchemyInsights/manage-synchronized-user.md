---
title: 동기화 된 사용자 관리
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
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777683"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="9dc6a-102">기본 전자 메일 주소를 설정 하거나, 사용자 특성을 변경 하거나, 동기화 된 사용자를 제거/삭제할 수 없음</span><span class="sxs-lookup"><span data-stu-id="9dc6a-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="9dc6a-103">환경에 대해 디렉터리 동기화를 사용 하도록 설정 된 경우에는 Microsoft 365 관리 센터를 사용 하 여 일부 사용자 또는 개체 특성을 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="9dc6a-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="9dc6a-104">동기화 된 사용자 및 모든 해당 특성을 완전히 관리 하려면 로컬 active directory 사용자 및 그룹 관리 콘솔 (adsiedit)을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="9dc6a-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="9dc6a-105">또는 다음과 같은 일반적인 예와 같이 powershell을 사용 하 여 동기화 된 사용자에 대 한 개별 사용자 또는 특성을 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9dc6a-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
