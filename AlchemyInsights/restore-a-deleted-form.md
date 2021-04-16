---
title: 삭제된 양식 복원
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2547"
- "9000672"
ms.openlocfilehash: 48018accc23a504c34b5469c198d6f29929d25c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809481"
---
# <a name="restore-a-deleted-form"></a><span data-ttu-id="5938e-102">삭제된 양식 복원</span><span class="sxs-lookup"><span data-stu-id="5938e-102">Restore a deleted form</span></span>

<span data-ttu-id="5938e-103">Microsoft Forms에서 사고로 양식을 삭제한 경우 복구할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5938e-103">If you deleted a form in Microsoft Forms by accident, you can recover it.</span></span> <span data-ttu-id="5938e-104">삭제된 양식의 소유자로 Microsoft Forms에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="5938e-104">Sign in to Microsoft Forms as the owner of the deleted form.</span></span> <span data-ttu-id="5938e-105">Recycle **Bin 을 선택한** 다음 복구할 양식을 선택하고 복원을 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="5938e-105">Select the **Recycle Bin**, then select the form you want to recover and select **Restore**.</span></span> <span data-ttu-id="5938e-106">복원되면 내 양식 **페이지로 돌아가기 화살표를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="5938e-106">Once restored, select the **Back to my Forms page** arrow.</span></span>

<span data-ttu-id="5938e-107">양식의 소유자만 복구할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5938e-107">Only the owner of the form can recover it.</span></span> <span data-ttu-id="5938e-108">양식 소유자의 계정을 사용하지 않도록 설정하거나 테넌트에서 제거한 경우 전역 관리자만 양식을 복구할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5938e-108">If form owner's account was disabled or removed from the tenant, only the Global Administrator can recover the form.</span></span> <span data-ttu-id="5938e-109">복원을 수행하려면 전역 관리자에게 Forms 라이선스가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5938e-109">The Global Administrator must have a Forms license to perform a restore.</span></span> <span data-ttu-id="5938e-110">사용자 계정이 사용하지 않도록 설정되거나 테넌트에서 제거된 후 30일 이내에 만들어진 양식만 복원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5938e-110">Only forms created within 30 days of the user account being disabled or removed from the tenant can be restored.</span></span>

<span data-ttu-id="5938e-111">테넌트의 전역 관리자인 경우 삭제되거나 사용하지 않도록 설정한 계정에서 양식을 복구하려면 [전자 메일 주소]를 다음 URL에서 삭제되거나 사용하지 않도록 설정한 사용자의 전자 메일 주소로 **https://forms.office.com/Pages/delegatepage.aspx?originalowner= 바꾸세요. [전자** 메일 주소] 예를 들어 전자 메일 주소가 johndoe@contoso.com URL은 입니다. **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com**</span><span class="sxs-lookup"><span data-stu-id="5938e-111">If you are the Global Administrator of the tenant, and you want to recover a form from an account that was deleted or disabled, replace [email address] with the email address of the deleted or disabled user in the following URL: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=[email address]** For example, if your email address is johndoe@contoso.com, the URL would be: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com**.</span></span> 

<span data-ttu-id="5938e-112">사용자의 삭제된 양식에 액세스할 수 있는 경우 이동할 양식을 선택한 다음 양식 동작 이동 을  >  **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="5938e-112">Once you have access to the user's deleted forms, select the form you want to move, and then select **More Form Actions** > **Move**.</span></span>

<span data-ttu-id="5938e-113">양식이 삭제되고 사용자가 조직에서 제거된 양식을 복구하려면 전역 관리자가 사용자를 복구하고 해당 사용자의 암호를 다시 설정한 다음 해당 사용자로 로그인한 동안 해당 양식에 액세스하여 다른 활성 사용자로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5938e-113">If you want to recover a form where it was deleted and the user was removed from the organization, a Global Administrator can choose to recover the user, reset the password for that user, and then while logged in as that user, access the form to move it to another active user.</span></span> 