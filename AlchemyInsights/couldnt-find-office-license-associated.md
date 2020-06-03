---
title: Office 앱을 수정 하면 office 라이선스 연결 된 메시지를 찾을 수 없음
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 887be4bee2bd1562bdc3b29783e9deafe47d8d57
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505873"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="72196-102">Office 앱 "연결 된 office 라이선스를 찾을 수 없습니다." 메시지를 수정 합니다.</span><span class="sxs-lookup"><span data-stu-id="72196-102">Fixing the Office apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="72196-103">이 메시지가 표시 되 면 다음을 시도해 보세요.</span><span class="sxs-lookup"><span data-stu-id="72196-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="72196-104">방화벽, 바이러스 백신 소프트웨어 및 프록시 설정을 확인 하 여 Office 앱에 대 한 인터넷 액세스를 차단 하 고 있지 않은지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="72196-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="72196-105">[Microsoft 365 url 및 IP 주소 범위](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="72196-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="72196-106">영향을 받는 사용자의 Office 라이선스를 제거 하 고 [다시 할당](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) 합니다.</span><span class="sxs-lookup"><span data-stu-id="72196-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="72196-107">Office 앱을 열고 기존 사용자 계정에서 [로그 아웃](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) 합니다.</span><span class="sxs-lookup"><span data-stu-id="72196-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="72196-108">Windows 설정 > **계정**  >  **전자 메일 & 계정**으로 이동 하 여 영향을 받는 계정을 제외한 모든 작업 계정을 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="72196-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="72196-109">Windows **설정 >으로**이동 하 여  >  **회사 또는 학교에 액세스**하 고, 영향을 받는 계정을 제외한 모든 작업 계정을 끊으십시오.</span><span class="sxs-lookup"><span data-stu-id="72196-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="72196-110">Office 정품 인증 상태 초기화</span><span class="sxs-lookup"><span data-stu-id="72196-110">Reset the Office activation state.</span></span> <span data-ttu-id="72196-111">[방법을 알아보세요](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="72196-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="72196-112">영향을 받는 사용자 계정을 사용 하 여 [로그인](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) 합니다.</span><span class="sxs-lookup"><span data-stu-id="72196-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="72196-113">문제 해결 솔루션에 대 한 자세한 내용은 [Office에서 허가 되지 않은 제품 및 정품 인증 오류](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="72196-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>