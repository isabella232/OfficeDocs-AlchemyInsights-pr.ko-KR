---
title: 도메인에 가입된 장치를 사용하여 조건부 액세스에서 차단되는 경우
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965466"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="83ba2-102">도메인에 가입된 장치를 사용하여 조건부 액세스에서 차단되는 경우</span><span class="sxs-lookup"><span data-stu-id="83ba2-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="83ba2-103">**권장 도구**</span><span class="sxs-lookup"><span data-stu-id="83ba2-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="83ba2-104">[장치 등록 문제 도구](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - 가장 일반적인 장치 등록 문제를 해결하는 데 도움이 되는 도구입니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="83ba2-105">[장치 등록 연결 스크립트 테스트](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - 장치가 시스템 계정 아래에 있는 장치 등록 끝점에 액세스할 수 있는지를 확인하는 데 도움이 되는 스크립트입니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="83ba2-106">[Azure AD 장치 정리 스크립트](https://github.com/mzmaili/AzureADDeviceCleanup) - 환경에서 오래된 장치를 검색하고 관리할 수 있는 스크립트입니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="83ba2-107">다음은 도메인(하이브리드 Azure AD)에 가입된 장치에서 조건부 액세스에 실패하는 몇 가지 일반적인 이유입니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="83ba2-108">**장치에 Azure AD PRT가 없음** - 장치에 Azure AD 기본 새로 고침 토큰(PRT)이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="83ba2-109">PRT에 대한 자세한 정보는 이 [문서](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="83ba2-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="83ba2-110">Azure AD PRT가 있는지 확인하려면 장치에서 `dsregcmd/status` 명령을 실행하고 "AzureAdPrt"가 "YES"인지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="83ba2-111">"AzureAdPrt"가 "NO"인 경우 다음을 검사합니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="83ba2-112">**AD FS 페더레이션 환경이 있으며 사용자의 홈 네트워크에서 액세스할 수 없는 경우**: 이 경우 엑스트라넷에서 "usernamemixed" 끝점에 액세스할 수 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="83ba2-113">AD FS가 VPN를 통해 제공되는 경우 사용자는 VPN에 연결하고 장치에 다시 로그인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="83ba2-114">자세한 정보는 이 [문서](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="83ba2-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="83ba2-115">**장치의 TPM에 문제가 있어 장치를 인증할 수 없는 경우**: "tpm.msc"를 확인하여 TPM 상태가 "Ready"인지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="83ba2-116">그렇지 않은 경우 `dsregcmd/leave`를 실행하고 장치가 Azure AD에 다시 참가하게 합니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="83ba2-117">그런 후에 다시 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-117">Then, try again.</span></span> <span data-ttu-id="83ba2-118">자세한 정보는 이 [문서](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="83ba2-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="83ba2-119">**WS-Trust 프로토콜을 지원하지 않는 제3자 ID 공급자를 사용하고 있습니다**.</span><span class="sxs-lookup"><span data-stu-id="83ba2-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="83ba2-120">문서에 설명된 대로 이 경우 하이브리드 Azure AD에 가입된 장치에서는 작동할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="83ba2-121">ID 공급자에게 지원을 요청하세요.</span><span class="sxs-lookup"><span data-stu-id="83ba2-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="83ba2-122">**사용자가 Windows 10 계정 없이 Chrome을 사용** 하거나 **Office 확장 Chrome에서 AAD에 가입 또는 하이브리드 AAD에 가입된 장치의 PRT를 자동으로 사용되지 않은 경우**: 이 경우 장치 기반 조건부 액세스 정책에 실패하게 되며 "등록되지 않은 장치" 오류 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="83ba2-123">Chrome 브라우저를 올바르게 사용하려면 SCCM 또는 Intune을 통해 "Windows 10 계정" 또는 "사용자의 Chrome 브라우저로 Office 확장"을 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="83ba2-124">자세한 정보는 이 [문서](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="83ba2-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="83ba2-125">원격으로 확장을 푸시할 수 없는 경우 사용자에게 위 확장 중 하나를 수동으로 설치하여 장치 기반 조건부 액세스의 기반이 되는 응용 프로그램에 액세스하도록 알립니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="83ba2-126">자세한 정보는 이 [문서](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="83ba2-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="83ba2-127">**장치가 올바르게 하이브리드 Azure AD에 조인됐지만, Azure AD Connect 또는 Azure Portal의 동기화 변경 사항으로 인해 장치가 우연히 삭제되거나 비활성화된 경우**: 이 경우 장치에서 "AzureAdJoined" 및 "PRT" 상태가 유효한 것으로 표시되어도 장치 개체가 더 이상 완전히 가입된 장치로 인식되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="83ba2-128">이 문제를 해결하기 위해 영향을 받는 장치에서 `dsregcmd/leave`를실행한 다음 Azure AD에 다시 연결합니다.</span><span class="sxs-lookup"><span data-stu-id="83ba2-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="83ba2-129">자세한 정보는 이 [문서](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="83ba2-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="83ba2-130">장치가 Windows 10, 1809 업데이트이며 VPN/클라우드 프록시를 사용하고 "AzureAdPrt" 상태와 관련된 문제가 표시되거나 앱에 SSO 문제(PRT가 있음에도 Outlook이 사서함에 연결되지 않음)가 있는 경우 이번 패치 [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) 또는 4월 누적 업데이트 [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6)를 통해 해당 컴퓨터에 PRT 오류를 방지하세요.</span><span class="sxs-lookup"><span data-stu-id="83ba2-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















