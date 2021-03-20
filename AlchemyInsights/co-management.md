---
title: 공동 관리
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: a10f2d9ee8617cf194c61492be69064d53242318
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50896801"
---
# <a name="co-management"></a><span data-ttu-id="38726-102">공동 관리</span><span class="sxs-lookup"><span data-stu-id="38726-102">Co-management</span></span>

<span data-ttu-id="38726-103">**Config Manager 하이브리드에서 Intune으로 마이그레이션하기 위한 선행 구성**</span><span class="sxs-lookup"><span data-stu-id="38726-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="38726-104">이 [문서를 검토합니다.](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid)</span><span class="sxs-lookup"><span data-stu-id="38726-104">Review [this article](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid).</span></span>
- <span data-ttu-id="38726-105">[사용자에게 Intune 라이선스를 추가합니다.](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign)</span><span class="sxs-lookup"><span data-stu-id="38726-105">[Add an Intune license to your users](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign).</span></span>
- <span data-ttu-id="38726-106">공동 관리를 구성할 때 [에지](https://www.microsoft.com/edge) 브라우저를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="38726-106">Use the [Edge browser](https://www.microsoft.com/edge) when configuring Co-management.</span></span>

<span data-ttu-id="38726-107">단계별 공동 관리 설치 환경은 에서 찾을 수 [있습니다.](https://admin.microsoft.com/AdminPortal/Home?#/modernonboarding/comanagesetupguide)</span><span class="sxs-lookup"><span data-stu-id="38726-107">A guided, step-by-step Co-management setup experience can be found [here](https://admin.microsoft.com/AdminPortal/Home?#/modernonboarding/comanagesetupguide).</span></span>

<span data-ttu-id="38726-108">**Intune 관리 장치에 Config Manager 클라이언트를 설치하는 방법**</span><span class="sxs-lookup"><span data-stu-id="38726-108">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="38726-109">[Intune MDM 관리 Windows 장치를 참조합니다.](https://docs.microsoft.com/mem/configmgr/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm)</span><span class="sxs-lookup"><span data-stu-id="38726-109">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/mem/configmgr/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="38726-110">**MDM 기관을 변경하려는 경우 어떻게 하나요?**</span><span class="sxs-lookup"><span data-stu-id="38726-110">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="38726-111">MDM 기관은 지원 사례를 열지 않고 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38726-111">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="38726-112">MDM 기관 변경을 지원하기 위해 다음 설명서를 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="38726-112">Please review the following documentation to assist in changing your MDM authority:</span></span>

- [<span data-ttu-id="38726-113">MDM Authority를 Configuration Manager에서 Intune 독립 실행형으로 변경</span><span class="sxs-lookup"><span data-stu-id="38726-113">Change MDM Authority from Configuration Manager to Intune standalone</span></span>](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid)
- [<span data-ttu-id="38726-114">MDM 기관을 Intune 독립 실행형에서 Configuration Manager로 변경</span><span class="sxs-lookup"><span data-stu-id="38726-114">Change MDM authority from Intune standalone to Configuration Manager</span></span>](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid)
