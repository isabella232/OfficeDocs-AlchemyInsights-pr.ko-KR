---
title: 2681 Microsoft 365의 공격 시뮬레이터
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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801557"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="992c5-102">Microsoft 365의 공격 시뮬레이터</span><span class="sxs-lookup"><span data-stu-id="992c5-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="992c5-103">공격 시뮬레이터가 누락 되었습니까?</span><span class="sxs-lookup"><span data-stu-id="992c5-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="992c5-104">Attack 시뮬레이터 **에는 Microsoft Defender For Office 365 계획 2 (ATP 계획 2)** 또는 **Office 365 Enterprise E5** 가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="992c5-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5** .</span></span> <span data-ttu-id="992c5-105">Attack 시뮬레이터는 Microsoft Defender for Office 365 계획 1 (ATP 계획 1), Office 365 Enterprise E3 또는 기타 Microsoft 365 앱 구독에 포함 되어 **있지** 않습니다.</span><span class="sxs-lookup"><span data-stu-id="992c5-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="992c5-106">시뮬레이트된 공격을 시작 하는 데 사용 하는 계정에는 전역 관리자 또는 보안 관리자 권한 및 MFA (multi-factor authentication)가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="992c5-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="992c5-107">공격 시뮬레이터 요구 사항에 대 한 자세한 내용은 [이 항목](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="992c5-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="992c5-108">**무작위 암호** 공격 시뮬레이션에 대해 알아야 할 중요 한 사항은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="992c5-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="992c5-109">대상 계정에 MFA를 사용 하 고 암호가 올바르게 추측 되 면 해당 계정에 손상 된 것으로 표시 되지 않습니다 (두 번째 인증 요인은 불완전 함).</span><span class="sxs-lookup"><span data-stu-id="992c5-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="992c5-110">암호 파일의 크기는 10mb를 넘을 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="992c5-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="992c5-111">한 줄에 하나씩 암호를 사용 하 고 목록의 마지막 암호 다음에 빈 줄 (캐리지 리턴)을 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="992c5-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="992c5-112">**스피어 피싱** 연결 시뮬레이션에 대해 알아야 할 중요 한 사항은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="992c5-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="992c5-113">기본적으로 **피싱 로그인 서버 URL** 에는 사용자 지정 값을 제공할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="992c5-113">By design, you can't provide a custom value for **Phishing login server URL** .</span></span>

  - <span data-ttu-id="992c5-114">받는 사람이 [보고서 메시지 추가 기능을 사용](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) 하 여 피싱로 메시지를 보고 하는 경우 시뮬레이트된 공격 이므로 메시지에 대 한 알림을 받지 못할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="992c5-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="992c5-115">보고서: 시뮬레이트된 공격이 완료 되 면 **공격 세부 정보** 를 클릭 하 여 보고서를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="992c5-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="992c5-116">자세한 지침 및 Attack 시뮬레이터의 새로운 기능은 [Microsoft 365의 Attack 시뮬레이터](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="992c5-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
