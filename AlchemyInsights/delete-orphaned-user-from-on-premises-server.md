---
title: 온-프레미스 서버에서 분리 된 사용자 삭제
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45186130"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="308b4-102">온-프레미스 서버에서 분리 된 사용자 삭제</span><span class="sxs-lookup"><span data-stu-id="308b4-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="308b4-103">분리 된 사용자를 삭제하려면 다음 단계를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="308b4-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="308b4-104">[Azure Active Directory에서 하이브리드 ID가 무엇인가요?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)의 지침에 따라 디렉토리 동기화를 강제로 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="308b4-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="308b4-105">디렉토리 동기화를 확인하려면 [Azure Active Directory에서 하이브리드 ID가 무엇인가요?](https://technet.microsoft.com/library/jj151797.aspx)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="308b4-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="308b4-106">동기화 기능이 제대로 작동하지 않지만 활성 디렉토리 객체 삭제가 Azure AD에 전파되지 않는 경우 다음 Windows PowerShell cmdlets용 Azure Active Directory 모듈 중 하나를 사용하여 분리된 개체를 수동으로 제거하세요.</span><span class="sxs-lookup"><span data-stu-id="308b4-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="308b4-107">제거-MsolContact</span><span class="sxs-lookup"><span data-stu-id="308b4-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="308b4-108">제거-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="308b4-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="308b4-109">제거-MsolUser</span><span class="sxs-lookup"><span data-stu-id="308b4-109">Remove-MsolUser</span></span>

    <span data-ttu-id="308b4-110">예를 들어, 디렉토리 동기화를 사용하여 만들어진 분리된 사용자 ID john.smith@contoso.com를 제거하려면 cmdlet을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="308b4-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="308b4-111">제거-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="308b4-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>