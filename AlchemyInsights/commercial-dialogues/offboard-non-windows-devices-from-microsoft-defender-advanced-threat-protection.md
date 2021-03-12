---
title: Microsoft Defender ATP(Advanced Threat Protection)에서 비 Windows 장치 오프보딩
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736540"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="19964-102">Microsoft Defender ATP(Advanced Threat Protection)에서 비 Windows 장치 오프보딩</span><span class="sxs-lookup"><span data-stu-id="19964-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="19964-103">방법은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="19964-103">Here's how:</span></span>

1. <span data-ttu-id="19964-104">타사 설명서에 따라 Microsoft Defender ATP에서 타사 솔루션 연결을 끊습니다.</span><span class="sxs-lookup"><span data-stu-id="19964-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="19964-105">Azure Active Directory 테넌트에서 타사 솔루션에 대한 사용 권한을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="19964-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="19964-106">[Azure 포털](https://go.microsoft.com/fwlink/?linkid=2125612)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="19964-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="19964-107">모든 **서비스**  >  **Azure Active Directory** 엔터프라이즈 응용 프로그램을  >  **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="19964-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="19964-108">오프보드할 응용 프로그램을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="19964-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="19964-109">**삭제** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="19964-109">Select **Delete**.</span></span>

<span data-ttu-id="19964-110">자세한 내용은 비 Windows 장치 [오프보드를 참조합니다.](https://go.microsoft.com/fwlink/?linkid=2143630)</span><span class="sxs-lookup"><span data-stu-id="19964-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
