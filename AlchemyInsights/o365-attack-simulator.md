---
title: 2681 공격 시뮬레이터의 Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545732"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="faa61-102">공격 시뮬레이터를 Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="faa61-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="faa61-103">공격 시뮬레이터가 누락된 경우</span><span class="sxs-lookup"><span data-stu-id="faa61-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="faa61-104">공격 시뮬레이터를 사용하려면 **Microsoft Defender for Office 365** 요금제 2 또는 Office 365 Enterprise **필요합니다.**</span><span class="sxs-lookup"><span data-stu-id="faa61-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="faa61-105">공격 **시뮬레이터는** Microsoft Defender for Office 365 플랜 1, E3 Office 365 Enterprise 또는 모든 비즈니스용 Microsoft 365 앱 포함되어 있지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="faa61-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="faa61-106">시뮬레이트된 공격을 시작하려면 전역 관리자 또는 보안 관리자 권한 및 MFA(다단계 인증)가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="faa61-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="faa61-107">공격 시뮬레이터 요구 사항에 대한 자세한 내용은 이 [항목을 참조하세요.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="faa61-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="faa61-108">Brute Force **Password** 공격 시뮬레이션에 대해 알아야 할 중요한 사항:</span><span class="sxs-lookup"><span data-stu-id="faa61-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="faa61-109">대상 계정이 MFA를 사용하도록 설정한 경우 암호를 올바르게 추측한 경우 계정이 손상된 것으로 표시되지 않습니다(두 번째 인증 요소가 불완전합니다).</span><span class="sxs-lookup"><span data-stu-id="faa61-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="faa61-110">암호 파일은 10MB보다 클 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="faa61-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="faa61-111">한 줄에 하나의 암호를 사용하며 목록의 마지막 암호 다음에 빈 줄(캐리지 리턴)을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="faa61-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="faa61-112">스피어 피싱 연결 시뮬레이션에 대해 알아야 할 **중요한** 사항:</span><span class="sxs-lookup"><span data-stu-id="faa61-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="faa61-113">기본적으로 피싱 로그인 서버 URL에 대한 사용자 지정 값을 제공할 **수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="faa61-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="faa61-114">받는 사람이 보고서 [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) 메시지 추가 기능을 사용하여 메시지를 피싱으로 보고하는 경우 시뮬레이트된 공격이기 때문에 메시지에 대한 경고가 수신되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="faa61-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="faa61-115">보고서: 시뮬레이션된 공격이 완료되면 공격 **세부 정보를** 클릭하여 보고서를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="faa61-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="faa61-116">공격 시뮬레이터의 자세한 지침과 새로운 기능은 에서 [공격 시뮬레이터를 Microsoft 365.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="faa61-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
