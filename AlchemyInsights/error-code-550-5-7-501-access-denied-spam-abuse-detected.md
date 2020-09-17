---
title: 오류 코드 550 5.7.501 액세스 거부, 스팸 남용 감지 됨
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 6542450ca4d03daef4a7f63783d431d2091bc5e7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784061"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="42aa5-102">550 5.7.501 액세스 거부, 스팸 남용 감지 됨</span><span class="sxs-lookup"><span data-stu-id="42aa5-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="42aa5-103">일반적으로이 메시지는 사용자가 Microsoft 365에서 새 테 넌 트에 할당 된 *onmicrosoft.com* 도메인을 사용 하 여 IP 주소에서 전자 메일 메시지를 보낼 때 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="42aa5-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Microsoft 365.</span></span> <span data-ttu-id="42aa5-104">이 문제를 해결 하는 가장 쉬운 방법은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="42aa5-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="42aa5-105">[테 넌 트에 도메인을 추가](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain)합니다.</span><span class="sxs-lookup"><span data-stu-id="42aa5-105">[Add a domain to your tenant](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="42aa5-106">[사용자의 기본 전자 메일 주소](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) 를 방금 추가한 새 사용자 지정 도메인으로 변경 합니다.</span><span class="sxs-lookup"><span data-stu-id="42aa5-106">[Change your users' primary email address](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
