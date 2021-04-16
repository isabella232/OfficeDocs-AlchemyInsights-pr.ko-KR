---
title: Office를 정품 인증할 수 없습니다
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812578"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="87668-102">Office를 정품 인증할 수 없습니다</span><span class="sxs-lookup"><span data-stu-id="87668-102">Unable to activate Office</span></span>

- <span data-ttu-id="87668-103">구독 상태가 만료되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="87668-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="87668-104">Office 365 Business 혹은 Business Premium과 같은 클라이언트 라이선스를 허용하는 구독이 있는지 확인하고 [사용자에게 라이선스가 할당되어 있는지 확인](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide)합니다.</span><span class="sxs-lookup"><span data-stu-id="87668-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="87668-105">사용자가 라이선스가 할당된 동일한 계정으로 Office에 로그인하고 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="87668-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="87668-106">[Office 365 서비스 상태 페이지](https://docs.microsoft.com/office365/enterprise/view-service-health)를 보고 서비스에 알려진 문제가 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="87668-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="87668-107">방화벽, 백신 소프트웨어 및 프록시 설정이 Microsoft 365 앱의 인터넷 액세스를 차단하고 있지 않은지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="87668-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="87668-108">[Office 365 URL 및 IP 주소 범위](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL 및 IP 주소 범위")를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="87668-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="87668-109">**팁** Windows 컴퓨터에서 몇 가지 일반적인 Office 로그인 문제를 자동으로 진단하고 해결해드립니다.</span><span class="sxs-lookup"><span data-stu-id="87668-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="87668-110">자동화된 도구를 사용하려면 **[Office 365 지원 및 복구 도우미](https://aka.ms/SaRA-OfficeSignInScenario)** 를 다운로드하고 실행하십시오.</span><span class="sxs-lookup"><span data-stu-id="87668-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="87668-111">다음 정보를 사용하여 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="87668-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="87668-112">Office 앱을 열고 기존 사용자 계정을 [로그아웃](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)합니다.</span><span class="sxs-lookup"><span data-stu-id="87668-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="87668-113">Office 라이선스를 [제거](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) 및 [다시 할당](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)한 다음 영향을 받는 사용자 계정을 사용하여 [Office에 로그인](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)합니다.</span><span class="sxs-lookup"><span data-stu-id="87668-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="87668-114">[정품 인증 문제 해결사](https://aka.ms/SARA-OfficeActivation-Alchemy) 실행</span><span class="sxs-lookup"><span data-stu-id="87668-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="87668-115">Office 정품 인증 다시 설정</span><span class="sxs-lookup"><span data-stu-id="87668-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office 정품 인증 상태 재설정")
- [<span data-ttu-id="87668-116">Office의 온라인 복구 실행</span><span class="sxs-lookup"><span data-stu-id="87668-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="87668-117">추가적인 문제 해결 솔루션을 보려면 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="87668-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="87668-118">사용 허가되지 않은 제품 및 Office 정품 인증 오류</span><span class="sxs-lookup"><span data-stu-id="87668-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="87668-119">Office를 정품 인증할 때 "사용자 계정에 연결할 수 없습니다. 나중에 다시 시도해 보세요." 오류</span><span class="sxs-lookup"><span data-stu-id="87668-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)