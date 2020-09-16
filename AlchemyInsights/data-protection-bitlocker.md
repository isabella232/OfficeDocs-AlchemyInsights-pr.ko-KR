---
title: DataProtection-Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731245"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="6c84c-102">Intune을 사용 하 여 Bitlocker 암호화 사용</span><span class="sxs-lookup"><span data-stu-id="6c84c-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="6c84c-103">Intune Endpoint Protection 정책은 Windows 장치에 대 한 Bitlocker 암호화 설정을 구성 하는 데 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6c84c-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="6c84c-104">자세한 내용은 [Intune을 사용 하 여 장치를 보호 하기 위해 Windows 10 이상 설정을](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="6c84c-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="6c84c-105">Windows 10을 실행 하는 많은 최신 장치는 MDM 정책 응용 프로그램 없이 트리거되는 자동 Bitlocker 암호화를 지원 한다는 점을 알고 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="6c84c-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="6c84c-106">기본 설정이 아닌 설정을 구성 하면 정책 응용 프로그램에 영향을 줄 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6c84c-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="6c84c-107">자세한 내용은 다음 FAQ를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="6c84c-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="6c84c-108">Bitlocker 문제를 해결 하는 방법에 대 한 자세한 내용은 [Microsoft Intune에서 bitlocker 정책 문제 해결](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="6c84c-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="6c84c-109">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="6c84c-109">**FAQ**</span></span>

 <span data-ttu-id="6c84c-110">Q: Endpoint Protection 정책을 사용 하 여 장치 암호화를 지 원하는 Windows 버전은 무엇입니까?</span><span class="sxs-lookup"><span data-stu-id="6c84c-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="6c84c-111">A: Intune Endpoint Protection 정책의 설정은 [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)를 사용 하 여 구현 됩니다.</span><span class="sxs-lookup"><span data-stu-id="6c84c-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="6c84c-112">Windows의 일부 버전 또는 빌드에서는 Bitlocker CSP를 지원 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6c84c-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="6c84c-113">현재는 엔터프라이즈, 교육, 모바일, 모바일 Enterprise 및 Professional (빌드 1809 이상)과 같은 Windows 버전이 지원 됩니다.</span><span class="sxs-lookup"><span data-stu-id="6c84c-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="6c84c-114">Q: 암호화 방법 및 암호화 수준 (XTS-128)에 대 한 운영 체제 기본 설정을 사용 하 여 장치가 이미 Bitlocker로 암호화 된 경우 다른 설정의 정책을 적용 하는 경우 새 설정으로 드라이브의 암호화를 자동으로 트리거합니다?</span><span class="sxs-lookup"><span data-stu-id="6c84c-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="6c84c-115">A: 아니요.</span><span class="sxs-lookup"><span data-stu-id="6c84c-115">A: No.</span></span> <span data-ttu-id="6c84c-116">새 암호화 설정을 적용 하려면 먼저 드라이브의 암호를 해독 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="6c84c-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="6c84c-117">**참고:** Autopilot을 사용 하 여 등록 되는 장치의 경우, OOBE 중에 발생 하는 자동 암호화는 Intune 정책을 평가할 때까지 트리거되지 않으므로 운영 체제 기본값 대신 정책 기반 설정을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6c84c-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="6c84c-118">Q: Intune 정책 응용 프로그램의 결과로 장치가 암호화 되 면 해당 정책이 제거 될 때 암호가 해독 됩니까?</span><span class="sxs-lookup"><span data-stu-id="6c84c-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="6c84c-119">A: 암호화 관련 정책을 제거 해도 구성 된 드라이브의 암호 해독이 발생 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6c84c-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="6c84c-120">Q: Intune 준수 정책에서 Bitlocker가 사용 하도록 설정 되어 있지 않은 경우에도 디바이스에서이를 표시 하는 이유는 무엇 인가요?</span><span class="sxs-lookup"><span data-stu-id="6c84c-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="6c84c-121">A: Intune 준수 정책에서 "Bitlocker enabled" 설정은 DHA (Windows 디바이스 상태 증명) 클라이언트를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="6c84c-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="6c84c-122">이 클라이언트는 부팅 시에만 장치 상태를 측정 합니다.</span><span class="sxs-lookup"><span data-stu-id="6c84c-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="6c84c-123">따라서 Bitlocker 암호화를 완료 한 후 장치를 다시 부팅 하지 않으면 DHA 클라이언트 서비스가 Bitlocker가 활성 상태인 것으로 보고 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6c84c-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 