---
title: 암호 쓰기 저장이 작동하지 않습니다.
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232783"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="ca1aa-102">암호 쓰기 저장이 작동하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ca1aa-102">Password Writeback is not working</span></span>

<span data-ttu-id="ca1aa-103">**암호 쓰기 저장 구성에 문제가 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="ca1aa-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="ca1aa-104">암호 쓰기 저장은 고급 기능입니다.</span><span class="sxs-lookup"><span data-stu-id="ca1aa-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="ca1aa-105">라이선스 요구 사항을 이해해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca1aa-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="ca1aa-106">조직에 라이선스가 하나 이상 할당되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca1aa-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="ca1aa-107">**클라우드 전용 사용자** - 모든 Office 365(O365) 유료 SKU 또는 Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="ca1aa-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="ca1aa-108">**클라우드 및/또는 프레미스** 사용자 - Azure AD Premium P1 또는 P2, EMS(Enterprise Mobility + Security) 또는 SPE(Secure Productive Enterprise)</span><span class="sxs-lookup"><span data-stu-id="ca1aa-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="ca1aa-109">라이선스 요구 사항에 대한 자세한 내용은 Azure AD 셀프 서비스 암호 재설정에 대한 [라이선스 요구 사항을 참조하세요.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="ca1aa-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="ca1aa-110">적절한 라이선스 중 하나를 사용하려면 관리자 계정과 테스트 사용자 계정이 하나 이상 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ca1aa-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="ca1aa-111">암호 쓰기 저장이 작동하려면 Azure AD Connect를 주 도메인 컨트롤러 에뮬레이터에 연결해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca1aa-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="ca1aa-112">Active Directory 동기화 커넥터의 속성을 마우스 오른쪽 단추로  클릭한 다음 디렉터리 파티션 구성을 선택하여 기본 도메인 컨트롤러를 사용하도록 Azure AD Connect를 구성할 **수 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="ca1aa-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="ca1aa-113">그런 다음 도메인  컨트롤러 연결 설정 섹션을 찾아 기본 설정 도메인 컨트롤러만 사용하는 확인란을 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="ca1aa-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="ca1aa-114">기본 설정 DC가 PDC 에뮬레이터가 아닌 경우 Azure AD Connect는 여전히 암호 쓰기 저장을 위해 PDC에 연결합니다.</span><span class="sxs-lookup"><span data-stu-id="ca1aa-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="ca1aa-115">암호 재설정이 테넌트에서 구성되고 사용하도록 설정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ca1aa-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="ca1aa-116">자세한 내용은 사용자가 Azure AD 암호를 재설정할 수 있도록 [설정하는 기능을 참조하세요.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="ca1aa-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="ca1aa-117">암호 쓰기 저장을 사용하도록 설정하는 데 사용되는 관리자 계정이 클라우드 관리자 계정(클라우드 관리자 계정이 아닌 Azure AD에서 생성)으로 설정되어 있는지 확인</span><span class="sxs-lookup"><span data-stu-id="ca1aa-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="ca1aa-118">최신 서비스 팩이 설치된 Windows Server 2008 R2, Windows Server 2012 또는 Windows Server 2012 R2를 실행하는 단일 또는 다중 포리스트 AD Windows Server 2012 배포가 있는 경우</span><span class="sxs-lookup"><span data-stu-id="ca1aa-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="ca1aa-119">Azure AD Connect 도구가 설치되어 있으며 클라우드와의 동기화를 위해 AD 환경을 준비했습니다.</span><span class="sxs-lookup"><span data-stu-id="ca1aa-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="ca1aa-120">암호 쓰기 저장을 테스트하기 전에 먼저 Azure AD Connect의 AD 및 Azure AD에서 전체 가져오기 및 전체 동기화를 완료해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca1aa-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="ca1aa-121">자세한 내용은 Azure AD Connect에서 전체 동기화 및 전체 가져오기 방법을 [참조하세요.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="ca1aa-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="ca1aa-122">**암호 쓰기 저장 연결에 문제가 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="ca1aa-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="ca1aa-123">최신 버전의 [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594) 다운로드 및 사용</span><span class="sxs-lookup"><span data-stu-id="ca1aa-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="ca1aa-124">방화벽 구성: Azure AD Connect 도구(1.1.443 이상)에는 다음에 대한 아웃바운드 **HTTPS** 액세스가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="ca1aa-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="ca1aa-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ca1aa-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="ca1aa-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="ca1aa-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="ca1aa-127">2~3분 이상 유휴 연결을 유지하도록 허용</span><span class="sxs-lookup"><span data-stu-id="ca1aa-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="ca1aa-128">**여전히 암호 쓰기 저장에 문제가 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="ca1aa-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="ca1aa-129">여전히 문제가 있는 경우 Azure AD Connect 도구에서 암호 쓰기 저장 서비스를 사용하도록 설정하고 다시 사용하도록 설정하십시오.</span><span class="sxs-lookup"><span data-stu-id="ca1aa-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="ca1aa-130">자세한 내용은 암호 쓰기 저장을 사용하지 않도록 설정하고 [다시 사용하도록 설정하는 방법을 참조하세요.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="ca1aa-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
