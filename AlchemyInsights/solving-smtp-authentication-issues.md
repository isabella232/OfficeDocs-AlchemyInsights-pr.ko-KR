---
title: SMTP 인증 문제 해결
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737995"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="25779-102">SMTP 인증 문제 해결</span><span class="sxs-lookup"><span data-stu-id="25779-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="25779-103">SMTP 전자 메일을 보내고 클라이언트나 응용 프로그램을 사용하여 인증할 때 5.7.57 또는 5.7.3 오류가 발생하는 경우, 다음과 같은 몇 가지 사항을 확인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="25779-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="25779-104">테넌트 또는 사용하려는 사서함에서 인증된 SMTP 전송이 사용하도록 설정되지 않았을 수 있습니다(두 설정 모두 확인).</span><span class="sxs-lookup"><span data-stu-id="25779-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="25779-105">자세한 내용은 [인증된 클라이언트 SMTP 제출 사용 또는 사용 안 함](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="25779-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="25779-106">[Azure 보안 기본값](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)을 테넌트에 사용할 수 있는지 확인합니다. 이 기능을 사용할 수 있는 경우 기본 인증(레거시라고도 함. 이는 사용자 이름과 암호를 사용함)을 사용하는 SMTP 인증에 실패합니다.</span><span class="sxs-lookup"><span data-stu-id="25779-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
