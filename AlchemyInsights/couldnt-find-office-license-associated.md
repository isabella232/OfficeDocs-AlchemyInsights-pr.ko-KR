---
title: Microsoft 365 앱 수정 Office 라이선스 관련 메시지를 찾을 수 없습니다.
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816494"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="3c9be-102">Microsoft 365 앱 "연결된 Office 라이선스를 찾을 수 없습니다." 메시지 수정</span><span class="sxs-lookup"><span data-stu-id="3c9be-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="3c9be-103">이 메시지를 받으면 다음을 시도해 보아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3c9be-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="3c9be-104">방화벽, 바이러스 백신 소프트웨어 및 프록시 설정을 확인하여 Microsoft 365 앱에 대한 인터넷 액세스를 차단하지 않는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="3c9be-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="3c9be-105">[Microsoft 365 URL 및 IP 주소 범위를 참조하세요.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="3c9be-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="3c9be-106">영향을 받는 사용자에 대한 [Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) 라이선스를 제거하고 다시 배포합니다.</span><span class="sxs-lookup"><span data-stu-id="3c9be-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="3c9be-107">Office 앱을 [열고](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) 기존 사용자 계정에서 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="3c9be-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="3c9be-108">Windows 설정 > **계정** 전자 & 계정으로 이동하고 영향을 받는 계정을 제외한 모든 직장 계정을  >  제거합니다.</span><span class="sxs-lookup"><span data-stu-id="3c9be-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="3c9be-109">Windows 설정 > **계정** 직장 또는 학교 액세스로 이동하고 영향을 받는 계정을 제외한 모든 직장 계정의 연결을  >  끊습니다.</span><span class="sxs-lookup"><span data-stu-id="3c9be-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="3c9be-110">Office 정품 인증 상태 초기화</span><span class="sxs-lookup"><span data-stu-id="3c9be-110">Reset the Office activation state.</span></span> <span data-ttu-id="3c9be-111">[방법을 알아보세요](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="3c9be-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="3c9be-112">[영향을 받는](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) 사용자 계정을 사용하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="3c9be-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="3c9be-113">추가 문제 해결 방법은 Office의 라이선스가 없는 제품 [및 정품 인증 오류를 참조하세요.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="3c9be-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>