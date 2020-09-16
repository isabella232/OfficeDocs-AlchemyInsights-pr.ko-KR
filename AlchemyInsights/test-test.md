---
title: SharePoint Online 용어 저장소에서 누락 된 용어
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750457"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="2d6f3-102">Intune을 사용 하 여 Bitlocker 암호화 사용</span><span class="sxs-lookup"><span data-stu-id="2d6f3-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="2d6f3-103">Intune Endpoint Protection 정책을 사용 하 여 Windows10 (이상) 설정에 설명 된 대로 Windows 장치에 대 한 Boitlocker 암호화 설정을 구성 하 여 Intune을 사용 하는 장치 보호</span><span class="sxs-lookup"><span data-stu-id="2d6f3-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="2d6f3-104">Windows 10을 실행 하는 많은 최신 장치는 MDM 정책 응용 프로그램 없이 트리거되는 자동 bitlocker 암호화를 지원 한다는 점을 알고 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d6f3-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="2d6f3-105">이렇게 하지 않으면 기본 설정이 아닌 설정을 구성 하는 경우 정책 응용 프로그램에 영향을 줄 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d6f3-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="2d6f3-106">자세한 내용은 FAQ를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="2d6f3-106">See FAQ for more detail.</span></span>


<span data-ttu-id="2d6f3-107">FAQ   Q: 어떤 버전의 Windows에서 Endpoint Protection 정책을 사용 하 여 장치 암호화를 지원 하나요?</span><span class="sxs-lookup"><span data-stu-id="2d6f3-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="2d6f3-108"> A: Intune Endpoint Protection 정책의 설정은 Bitlocker CSP를 사용 하 여 구현 됩니다.</span><span class="sxs-lookup"><span data-stu-id="2d6f3-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="2d6f3-109">모든 에디션 및 Windows 빌드가 Bitlocker CSP를 지 원하는 것은 아닙니다. 
     </span><span class="sxs-lookup"><span data-stu-id="2d6f3-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="2d6f3-110">현재 Windows Edition: Enterprise; 교육, 모바일, 모바일 엔터프라이즈 및 전문가 (빌드 1809에서)가 지원 됩니다.</span><span class="sxs-lookup"><span data-stu-id="2d6f3-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="2d6f3-111">Q: 암호화 방법에 대 한 운영 체제 기본 설정을 사용 하 여 장치가 이미 Bitlocker로 암호화 되어 있고 암호화 수준 (XTS-128)이 다른 설정의 정책을 적용 하는 경우 새 설정으로 드라이브의 다시 암호화를 자동으로 트리거합니다?</span><span class="sxs-lookup"><span data-stu-id="2d6f3-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="2d6f3-112">A: 아니요.</span><span class="sxs-lookup"><span data-stu-id="2d6f3-112">A: No.</span></span> <span data-ttu-id="2d6f3-113">새 암호화 설정을 적용 하려면 드라이브를 먼저 해독 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d6f3-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="2d6f3-114">Autopilot을 사용 하 여 등록 된 장치에 대해 OOBE 중에 발생 하는 자동 암호화는 운영 체제 기본값 대신 정책 기반 설정을 사용할 수 있도록 Intune 정책을 평가할 때까지 트리거되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2d6f3-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="2d6f3-115">Q: Intune 정책 응용 프로그램의 결과로 장치가 암호화 되 면 해당 정책이 제거 될 때 암호가 해독 됩니까?</span><span class="sxs-lookup"><span data-stu-id="2d6f3-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="2d6f3-116">A: 암호화 관련 정책을 제거 해도 구성 된 드라이브의 암호 해독이 발생 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2d6f3-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="2d6f3-117">Q: intune 준수 정책에서 내 장치에 "Bitlocker 사용"이 설정 되어 있지 않은 것으로 표시 되는 이유는 무엇 인가요?</span><span class="sxs-lookup"><span data-stu-id="2d6f3-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="2d6f3-118">A: intune 준수 정책에서 "Bitlocker enabled" 설정은 DHA (Windows 디바이스 상태 증명) 클라이언트를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d6f3-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="2d6f3-119">이 클라이언트는 부팅 시에만 장치 상태를 측정 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d6f3-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="2d6f3-120">따라서 bitlocker 암호화가 완료 된 후 장치가 다시 부팅 되지 않은 경우 DHA 클라이언트 서비스가 bitlocker를 활성 상태로 보고 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2d6f3-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>