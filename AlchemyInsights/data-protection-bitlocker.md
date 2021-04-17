---
title: DataProtection - Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815621"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="bff28-102">Intune을 사용하여 Bitlocker 암호화 사용</span><span class="sxs-lookup"><span data-stu-id="bff28-102">Enabling Bitlocker encryption with Intune</span></span>

<span data-ttu-id="bff28-103">Intune 끝점 보호 정책을 사용하여 Windows 장치에 대한 Bitlocker 암호화 설정을 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bff28-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="bff28-104">자세한 내용은 [Intune을](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)사용하여 장치를 보호하기 위한 Windows 10 이상 설정을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="bff28-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>

<span data-ttu-id="bff28-105">엔드포인트 보호 정책 외에도 디바이스의 암호화 상태에 대한 자세한 보기를 제공하는 암호화 보고서도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bff28-105">In addition to the Endpoint Protection Policy there is also an Encryption Report which provides a more detailed view of the encryption status for devices.</span></span> <span data-ttu-id="bff28-106">이 보고서는 장치 및 모니터링의 MEM **포털에서**> 다음 구성 **선택** 암호화 [보고서에서 액세스할 수 있습니다.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)</span><span class="sxs-lookup"><span data-stu-id="bff28-106">This report can be accessed from the MEM portal under **Devices > Monitor**, and then under **Configuration** select [Encryption report](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).</span></span>

<span data-ttu-id="bff28-107">Bitlocker를 예상대로 사용하도록 설정하지 못하거나 Bitlocker를 사용하도록 설정하는 데 사용되는 프로필이 오류 상태인 경우 암호화 보고서를 검토하여 동작이 발생하는 이유를 더 잘 이해하세요.</span><span class="sxs-lookup"><span data-stu-id="bff28-107">If you find that Bitlocker fails to be enabled as expected or that the profile being used to enable Bitlocker is in an error state, please review the encryption report to get a better understanding of why the behavior is occurring.</span></span>

<span data-ttu-id="bff28-108">다양한 암호화 상태 값을 포함하여 보고서를 해석하는 방법에 대한 자세한 내용은 Intune을 사용하여 장치 암호화 [모니터링을 참조하세요.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)</span><span class="sxs-lookup"><span data-stu-id="bff28-108">To find details on how to interpret the report including the various encryption status values, see [Monitor device encryption with Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).</span></span>

<span data-ttu-id="bff28-109">Windows 10을 실행하는 많은 새 디바이스는 MDM 정책을 적용하지 않고 트리거되는 자동 Bitlocker 암호화를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="bff28-109">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="bff28-110">기본 설정이 아닌 설정이 구성된 경우 정책 적용에 영향을 줄 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bff28-110">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="bff28-111">자세한 내용은 다음 FAQ를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="bff28-111">See the following FAQ for more detail.</span></span>

<span data-ttu-id="bff28-112">BitLocker 문제 해결에 대한 자세한 내용은 [Microsoft Intune에서 BitLocker 정책 문제 해결을 참조하세요.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)</span><span class="sxs-lookup"><span data-stu-id="bff28-112">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="bff28-113">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="bff28-113">**FAQ**</span></span>

<span data-ttu-id="bff28-114">Q: Endpoint Protection 정책을 사용하여 장치 암호화를 지원하는 Windows 버전은 무엇입니까?</span><span class="sxs-lookup"><span data-stu-id="bff28-114">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="bff28-115">A: Intune 끝점 보호 정책의 설정은 [Bitlocker CSP를 사용하여 구현됩니다.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)</span><span class="sxs-lookup"><span data-stu-id="bff28-115">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="bff28-116">Windows의 모든 버전 또는 빌드는 Bitlocker CSP를 지원하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="bff28-116">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="bff28-117">Q: 최종 사용자 조작 없이 장치에서 Bitlocker를 사용하도록 설정하는 방법</span><span class="sxs-lookup"><span data-stu-id="bff28-117">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="bff28-118">A: 필요한 필수가 충족된 경우 Intune을 통해 Bitlocker "자동 암호화"를 사용하도록 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bff28-118">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="bff28-119">다음의 doc: [Silently Enable Bitlocker Encryption에서](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)자동 암호화를 사용하도록 설정하려면 장치 요구 사항 및 예제 정책 설정에 대한 세부 정보를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="bff28-119">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="bff28-120">Q: 장치가 암호화 방법 및 암호화 강도에 대한 OS 기본 설정(XTS-AES-128)을 사용하여 이미 Bitlocker로 암호화된 경우 다른 설정을 사용하는 정책을 적용하면 새 설정으로 드라이브의 다시 암호화가 자동으로 트리거하나요?</span><span class="sxs-lookup"><span data-stu-id="bff28-120">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="bff28-121">A: 아니요.</span><span class="sxs-lookup"><span data-stu-id="bff28-121">A: No.</span></span> <span data-ttu-id="bff28-122">새 암호화 설정을 적용하려면 먼저 드라이브의 암호를 해독해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="bff28-122">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="bff28-123">**참고:** Autopilot을 사용하여 등록하는 장치의 경우 Intune 정책이 평가될 때까지 OOBE 중에 발생하는 자동 암호화가 트리거되지 않습니다. 이렇게 하면 OS 기본값 대신 정책 기반 설정을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bff28-123">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="bff28-124">Q: Intune 정책이 적용된 결과로 장치가 암호화된 경우 해당 정책이 제거될 때 암호가 해독될 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="bff28-124">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="bff28-125">A: 암호화 관련 정책을 제거하면 구성된 드라이브의 암호 해독이 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="bff28-125">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="bff28-126">Q: Intune 규정 준수 정책은 장치가 Bitlocker를 사용하도록 설정되어 있지 않은 것으로 표시하는 이유는 무엇입니까?</span><span class="sxs-lookup"><span data-stu-id="bff28-126">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="bff28-127">A: Intune 준수 정책의 "Bitlocker 사용" 설정은 Windows DHA(장치 상태 스터스터) 클라이언트를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="bff28-127">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="bff28-128">이 클라이언트는 부팅 시 장치 상태만 측정합니다.</span><span class="sxs-lookup"><span data-stu-id="bff28-128">This client only measures device state at boot time.</span></span> <span data-ttu-id="bff28-129">따라서 Bitlocker 암호화가 완료된 후 장치를 다시 시작하지 않은 경우 DHA 클라이언트 서비스는 Bitlocker가 활성 상태인 것으로 보고하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="bff28-129">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 