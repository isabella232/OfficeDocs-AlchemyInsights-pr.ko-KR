---
title: Microsoft 365 앱에 로그인하는 문제
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
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833081"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="b428a-102">Microsoft 365 앱 수정 "죄송합니다. 조직의 다른 계정이 이미 로그인되어 있습니다." 메시지 수정</span><span class="sxs-lookup"><span data-stu-id="b428a-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="b428a-103">이 오류를 해결하려면 다음 단계를 수행하십시오.</span><span class="sxs-lookup"><span data-stu-id="b428a-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="b428a-104">Windows 설정 을 사용하여 영향을 받는 계정을 제외한 모든 작업 계정을 > **또는 학교에 액세스합니다.**</span><span class="sxs-lookup"><span data-stu-id="b428a-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="b428a-105">Windows [자격 증명 관리자를](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) 사용하여 Office 자격 증명 지우기</span><span class="sxs-lookup"><span data-stu-id="b428a-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="b428a-106">**참고:** Office 2016의 레지스트리 경로가 16.0으로 변경됩니다.</span><span class="sxs-lookup"><span data-stu-id="b428a-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="b428a-107">(예: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="b428a-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="b428a-108">Office 앱을 열고 파일  >  **계정 로그인**  >  **을 선택하세요.** 그런 다음 유효한 라이선스가 있는 사용자 계정을 사용하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="b428a-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="b428a-109">자세한 내용은 [Office의 계정](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b428a-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="b428a-110">Mac의 경우 [Mac용 Office 2016 앱에 로그인 할 수 없습니다](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b428a-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="b428a-111">자세한 내용은 [Office에서 "죄송합니다.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)조직의 다른 계정이 이미 이 컴퓨터에 로그인되어 있습니다."를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b428a-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>