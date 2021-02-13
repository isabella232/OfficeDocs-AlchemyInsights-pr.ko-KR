---
title: Microsoft Intune에 Microsoft Edge 추가
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50178000"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="50fe0-102">Microsoft Intune에 Microsoft Edge 추가</span><span class="sxs-lookup"><span data-stu-id="50fe0-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="50fe0-103">Windows 10용 Microsoft Edge를 배포, 구성, 모니터링 및 보호하려면 먼저 Microsoft Edge를 Microsoft Intune에 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="50fe0-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="50fe0-104">Intune은 Microsoft Edge 77 이상 버전을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="50fe0-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="50fe0-105">Intune은 Microsoft Edge의 기존 설치를 감지합니다.</span><span class="sxs-lookup"><span data-stu-id="50fe0-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="50fe0-106">Microsoft Edge가 사용자 컨텍스트에 설치되어 있으면 시스템 설치가 사용자 컨텍스트에서 설치를 덮어씁니다.</span><span class="sxs-lookup"><span data-stu-id="50fe0-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="50fe0-107">시스템 컨텍스트에 Microsoft Edge가 설치되어 있는 경우 설치 성공이 보고됩니다.</span><span class="sxs-lookup"><span data-stu-id="50fe0-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="50fe0-108">사용자 컨텍스트의 모든 채널에 대해 미리 설치된 Microsoft Edge 77 이상 버전은 시스템 컨텍스트에 설치된 Microsoft Edge로 덮어씁니다.</span><span class="sxs-lookup"><span data-stu-id="50fe0-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="50fe0-109">**필수 구성 요소**</span><span class="sxs-lookup"><span data-stu-id="50fe0-109">**Prerequisite**</span></span>

<span data-ttu-id="50fe0-110">Windows 10 버전 1709 이상 버전</span><span class="sxs-lookup"><span data-stu-id="50fe0-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="50fe0-111">**Intune에 Edge를 추가하기 위한 단계**</span><span class="sxs-lookup"><span data-stu-id="50fe0-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="50fe0-112">[Intune에서 앱 구성](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="50fe0-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="50fe0-113">[앱 정보 구성](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="50fe0-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="50fe0-114">[앱 설정 구성](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="50fe0-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="50fe0-115">[범위 태그(선택 사항) 선택](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="50fe0-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="50fe0-116">[앱 추가](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="50fe0-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="50fe0-117">추가 도움말을 확인하려면 [문제 해결](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="50fe0-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




