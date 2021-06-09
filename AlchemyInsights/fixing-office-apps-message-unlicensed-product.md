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
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798686"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="a65df-102">Office를 정품 인증할 수 없습니다</span><span class="sxs-lookup"><span data-stu-id="a65df-102">Unable to activate Office</span></span>

<span data-ttu-id="a65df-103">**참고**: 이전 버전의 Windows(예: Windows 7)를 사용하는 경우 TLS 1.2가 기본값으로 사용하도록 설정되어 있는지 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="a65df-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="a65df-104">자세한 내용은 [Windows의 WinHTTP에서 기본 보안 프로토콜로 TLS 1.1 및 TLS 1.2를 사용하도록 업데이트](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a65df-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="a65df-105">구독 상태가 만료되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="a65df-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="a65df-106">Office 365 Business 혹은 Business Premium과 같은 클라이언트 라이선스를 허용하는 구독이 있는지 확인하고 [사용자에게 라이선스가 할당되어 있는지 확인](/microsoft-365/admin/manage/assign-licenses-to-users)합니다.</span><span class="sxs-lookup"><span data-stu-id="a65df-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="a65df-107">사용자가 라이선스가 할당된 동일한 계정으로 Office에 로그인하고 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="a65df-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="a65df-108">[Office 365 서비스 상태 페이지](/office365/enterprise/view-service-health)를 보고 서비스에 알려진 문제가 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="a65df-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="a65df-p102">방화벽, 백신 소프트웨어 및 프록시 설정이 Microsoft 365 앱의 인터넷 액세스를 차단하고 있지 않은지 확인합니다. [Office 365 URL 및 IP 주소 범위](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL 및 IP 주소 범위")를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a65df-p102">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet. Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="a65df-111">**팁** Windows 컴퓨터에서 몇 가지 일반적인 Office 로그인 문제를 자동으로 진단하고 해결해드립니다.</span><span class="sxs-lookup"><span data-stu-id="a65df-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="a65df-112">자동화된 도구를 사용하려면 **[Office 365 지원 및 복구 도우미](https://aka.ms/SaRA-OfficeSignInScenario)** 를 다운로드하고 실행하십시오.</span><span class="sxs-lookup"><span data-stu-id="a65df-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="a65df-113">다음 정보를 사용하여 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="a65df-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="a65df-114">Office 앱을 열고 기존 사용자 계정을 [로그아웃](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)합니다.</span><span class="sxs-lookup"><span data-stu-id="a65df-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="a65df-115">Office 라이선스를 [제거](/microsoft-365/admin/manage/remove-licenses-from-users) 및 [다시 할당](/microsoft-365/admin/manage/assign-licenses-to-users)한 다음 영향을 받는 사용자 계정을 사용하여 [Office에 로그인](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)합니다.</span><span class="sxs-lookup"><span data-stu-id="a65df-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="a65df-116">[정품 인증 문제 해결사](https://aka.ms/SARA-OfficeActivation-Alchemy) 실행</span><span class="sxs-lookup"><span data-stu-id="a65df-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="a65df-117">Office 정품 인증 다시 설정</span><span class="sxs-lookup"><span data-stu-id="a65df-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office 정품 인증 상태 재설정")
- [<span data-ttu-id="a65df-118">Office의 온라인 복구 실행</span><span class="sxs-lookup"><span data-stu-id="a65df-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="a65df-119">추가적인 문제 해결 솔루션을 보려면 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a65df-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="a65df-120">사용 허가되지 않은 제품 및 Office 정품 인증 오류</span><span class="sxs-lookup"><span data-stu-id="a65df-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="a65df-121">Office를 정품 인증할 때 "사용자 계정에 연결할 수 없습니다. 나중에 다시 시도해 보세요." 오류</span><span class="sxs-lookup"><span data-stu-id="a65df-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)