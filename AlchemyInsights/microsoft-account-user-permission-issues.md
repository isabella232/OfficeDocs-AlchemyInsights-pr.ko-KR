---
title: 문제 해결-디렉터리에서 사용자를 찾을 수 없음
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725413"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="ac600-102">문제 해결-디렉터리에서 사용자를 찾을 수 없음</span><span class="sxs-lookup"><span data-stu-id="ac600-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="ac600-103">사용자가 디렉터리에서 "사용자를 찾을 수 없습니다." 라는 오류 메시지가 표시 되는 경우 문제 유형이 디렉터리에 없는 사용자 인 경우 다시 시도 하세요.</span><span class="sxs-lookup"><span data-stu-id="ac600-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="ac600-104">문제를 해결 하기 위해 다음 단계를 완료할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ac600-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="ac600-105">전자 메일 초대를 수락한 계정이 나중에 로그인 하는 데 사용 되는 것과 동일한 계정 인지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ac600-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="ac600-106">사용자가 초대를 수락 하 고 사이트에 로그인 하는 데 동일한 계정을 사용 하 고 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ac600-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="ac600-107">자세한 내용은 microsoft [계정을 </a> 365 관리 하기 위해 microsoft 계정의 별칭을 관리](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)하는 방법을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="ac600-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="ac600-108">사용자에 게 오류를 수신 하는 각 사이트로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="ac600-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="ac600-109">사이트 URL 끝에 "/_layouts/15/people.aspx/membershipgroupid = 0" (이중 따옴표 내)을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="ac600-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="ac600-110">예: https://< "contoso" sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 >.</span><span class="sxs-lookup"><span data-stu-id="ac600-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="ac600-111">목록에서 사용자를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="ac600-111">Select the user from the list.</span></span>

- <span data-ttu-id="ac600-112">리본에서 **사용자 권한 제거** 를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="ac600-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="ac600-113">사용자를 추가 하 고 사용자에 게 초대를 다시 보냅니다.</span><span class="sxs-lookup"><span data-stu-id="ac600-113">Add back the User and Resend the invite to the user.</span></span>

