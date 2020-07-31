---
title: 클라이언트 인증 인증서 배포 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509071"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="98761-102">클라이언트 인증 인증서 배포 문제 해결</span><span class="sxs-lookup"><span data-stu-id="98761-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="98761-103">Intune NDES/SCEP 및 PKCS/PFX 클라이언트 인증서 프로필은 사용자가 회사 리소스를 인증 하도록 허용하는 데 사용할 수 있는 Wifi, VPN, 전자 메일 등의 다른 프로필 유형과 함께 자주 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="98761-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="98761-104">해당 프로필 유형이 클라이언트 인증서 프로필에 연결되면, 해당 프로필 유형은 배포 성공 여부에 따라 달라집니다.</span><span class="sxs-lookup"><span data-stu-id="98761-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="98761-105">초기 인프라 설정과 클라이언트 인증서 프로필 관련 구성에는 종종 문제 해결이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="98761-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="98761-106">NDES 커넥터의 성공적인 설정을 위한 단계별 가이드 및 인증서 배포에 관한 문제를 격리하는 문제 해결 지침은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="98761-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="98761-107">Intune에서 SCEP를 지원하도록 인프라 구성</span><span class="sxs-lookup"><span data-stu-id="98761-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="98761-108">Microsoft Intune에서 SCEP 인증서 프로필 문제 해결에 대한 개요</span><span class="sxs-lookup"><span data-stu-id="98761-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="98761-109">참조된 Powershell 스크립트로 구성을 확인해보세요.</span><span class="sxs-lookup"><span data-stu-id="98761-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="98761-110">자세한 내용은 [Intune 인증서 커넥터 확인 스크립트](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="98761-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="98761-111">**기타 일반적인 문제**</span><span class="sxs-lookup"><span data-stu-id="98761-111">**Other common issues**</span></span>

<span data-ttu-id="98761-112">**NDES 커넥터 서버에 Intune 인증서 커넥터를 설치하려고 하면 ‘인증서 요청의 암호를 확인할 수 없습니다. 이미 사용되었을 수 있습니다. 이 요청과 함께 제출할 새 암호를 가져옵니다.’라는 메시지가 표시 됩니다.**</span><span class="sxs-lookup"><span data-stu-id="98761-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="98761-113">이 메시지는 사용자가 인증서 커넥터 설치를 관리자 권한으로 실행해야 함을 의미합니다.</span><span class="sxs-lookup"><span data-stu-id="98761-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="98761-114">일부 환경의 경우 Intune 인증서가 실행되는 서버에 프록시 서버를 사용하여 Intune에 연결해야 합니다. 따라서 인증서 커넥터에서 프록시를 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="98761-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="98761-115">경우에 따라 NDES 커넥터에서 구성된 프록시 설정을 무시하고 LocalSystem의 보안 컨텍스트를 실행하는 동안 프록시 설정을 구성해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="98761-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="98761-116">Internet Explorer를 시스템으로 실행하고 IE에서 프록시를 구성하여 이 문제를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="98761-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="98761-117">Intune 커넥터 서비스를 다시 시작하면 NDES 커넥터가 Intune에 연결됩니다.</span><span class="sxs-lookup"><span data-stu-id="98761-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="98761-118">**사용자 장치의 경우에는 NDES에서 더 이상 SCEP 인증서를 받을 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="98761-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="98761-119">NDES 서버에 발급되고 NDES 커넥터 설치 중에 지정된 클라이언트 인증 인증서가 만료되었거나 누락되었을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="98761-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="98761-120">해결할 문제:</span><span class="sxs-lookup"><span data-stu-id="98761-120">To resolve:</span></span> 
 
1. <span data-ttu-id="98761-121">NDES 커넥터를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="98761-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="98761-122">다음 세부 사항을 활용하여 새 클라이언트 인증 또는 서버 인증 인증서를 요청할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="98761-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="98761-123">주체 이름: CN=외부 fqdn</span><span class="sxs-lookup"><span data-stu-id="98761-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="98761-124">주제 대체 이름(둘 다 필수): DNS=외부 fqdn, DNS=내부 fqdn</span><span class="sxs-lookup"><span data-stu-id="98761-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="98761-125">새 인증서를 사용하여 NDES 커넥터를 다시 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="98761-125">Reinstall the NDES connector with the new certificate.</span></span>