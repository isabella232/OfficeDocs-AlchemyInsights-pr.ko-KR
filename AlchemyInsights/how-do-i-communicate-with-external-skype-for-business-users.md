---
title: 외부 비즈니스용 Skype 사용자와 통신 하는 방법
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
- "4000008"
- "2646"
- "1432"
ms.openlocfilehash: f5e1e597067efff58872a5f0080bb18c42af648e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47781865"
---
# <a name="allow-external-communications-with-skype-for-business"></a><span data-ttu-id="7f3f0-102">비즈니스용 Skype와의 외부 통신 허용</span><span class="sxs-lookup"><span data-stu-id="7f3f0-102">Allow external communications with Skype for Business</span></span> 

<span data-ttu-id="7f3f0-103">비즈니스용 Skype 사용자가 조직 외부의 사용자에 게 연락할 수 있도록 허용 하 시겠습니까?</span><span class="sxs-lookup"><span data-stu-id="7f3f0-103">Do you want to allow your Skype for Business users to contact users outside your organization?</span></span> <span data-ttu-id="7f3f0-104">[사용자가 외부 비즈니스용 Skype 사용자와 연락 하도록 허용을](https://docs.microsoft.com/skypeforbusiness/set-up-skype-for-business-online/allow-users-to-contact-external-skype-for-business-users)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="7f3f0-104">See [Allow users to contact external Skype for Business users](https://docs.microsoft.com/skypeforbusiness/set-up-skype-for-business-online/allow-users-to-contact-external-skype-for-business-users).</span></span>

<span data-ttu-id="7f3f0-105">외부 통신이 제대로 작동 하려면 DNS 레코드가 올바르게 설정 되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7f3f0-105">Your DNS records MUST be set up correctly for external communications to function properly.</span></span> <span data-ttu-id="7f3f0-106">공급자를 사용 하 여 DNS 레코드를 설정 하는 방법에 대 한 특정 지침이 있는지 확인 하려면 [여기](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions) 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7f3f0-106">Check [here](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions) to see if we have specific instructions on how to set DNS records with your provider.</span></span> 

<span data-ttu-id="7f3f0-107">비즈니스용 Skype 사용자만 Skype 소비자 사용자에 게 연락할 수 있도록 설정 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="7f3f0-107">Do you only want to enable your Skype for Business users to contact Skype consumer users?</span></span> <span data-ttu-id="7f3f0-108">자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7f3f0-108">See:</span></span>

- <span data-ttu-id="7f3f0-109">비즈니스용 [skype 사용자가 skype 연락처를 추가할 수 있도록](https://docs.microsoft.com/skypeforbusiness/set-up-skype-for-business-online/let-skype-for-business-users-add-skype-contacts)합니다.</span><span class="sxs-lookup"><span data-stu-id="7f3f0-109">[Let Skype for Business users add Skype contacts](https://docs.microsoft.com/skypeforbusiness/set-up-skype-for-business-online/let-skype-for-business-users-add-skype-contacts).</span></span> 

- <span data-ttu-id="7f3f0-110">[비즈니스용 Skype에서 연락처를 추가](https://support.office.com/article/add-a-contact-in-skype-for-business-89338023-2adf-4f5c-90b6-f8b6f72fadd1)합니다.</span><span class="sxs-lookup"><span data-stu-id="7f3f0-110">[Add a contact in Skype for Business](https://support.office.com/article/add-a-contact-in-skype-for-business-89338023-2adf-4f5c-90b6-f8b6f72fadd1).</span></span>


<span data-ttu-id="7f3f0-111">팀 사용자가 조직 외부의 사용자에 게 연락할 수 있도록 하려면 (비즈니스용 Skype 사용자 포함) [Microsoft 팀에서 외부 액세스 관리](https://docs.microsoft.com/microsoftteams/let-your-teams-users-communicate-with-other-people)를 검토 합니다.</span><span class="sxs-lookup"><span data-stu-id="7f3f0-111">If you want your Teams users to be able to contact users outside of your organization (including Skype for Business users), review [Manage external access in Microsoft Teams](https://docs.microsoft.com/microsoftteams/let-your-teams-users-communicate-with-other-people).</span></span> 