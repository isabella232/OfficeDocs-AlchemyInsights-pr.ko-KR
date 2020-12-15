---
title: Intune Win32 앱 배포
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366527"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="bf0a9-102">Intune Win32 앱 배포</span><span class="sxs-lookup"><span data-stu-id="bf0a9-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="bf0a9-103">Microsoft Intune을 사용하면 MSI와 .EXE를 비롯하여(이에 국한되지는 않음) Win32 응용 프로그램을 Windows 10 장치에 배포할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf0a9-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="bf0a9-104">사용되는 배포 메커니즘을 사용하려면 대상 장치에 IME(Intune 관리 확장)이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf0a9-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="bf0a9-105">Powershell 스크립트나 win32 응용 프로그램 배포를 사용자/장치에 대상 지정하면 IME가 자동으로 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="bf0a9-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="bf0a9-106">또한 다음을 포함하는 Win32 앱을 배포하는 데 충족되어야 하는 사전 필수 항목 집합이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf0a9-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="bf0a9-107">지원되는 플랫폼: Windows 10 버전 1607 이상(Enterprise, Pro, 및 Education 버전)입니다.</span><span class="sxs-lookup"><span data-stu-id="bf0a9-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="bf0a9-108">지원되는 아키텍처: x86 및 x64입니다.</span><span class="sxs-lookup"><span data-stu-id="bf0a9-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="bf0a9-109">장치 관리: AAD에서 조인하고 자동으로 등록됩니다(하이브리드 도메인 조인과 그룹 정책 자동 등록 포함).</span><span class="sxs-lookup"><span data-stu-id="bf0a9-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="bf0a9-110">응용 프로그램 패키지 형식: [Microsoft Win32 콘텐츠 Prep 도구](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)로 준비된 .**intunewin** 파일입니다.</span><span class="sxs-lookup"><span data-stu-id="bf0a9-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="bf0a9-111">제한 사항:</span><span class="sxs-lookup"><span data-stu-id="bf0a9-111">Limitations:</span></span>
    - <span data-ttu-id="bf0a9-112">최대 크기: 8GB입니다.</span><span class="sxs-lookup"><span data-stu-id="bf0a9-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="bf0a9-113">지원되지 않는 아키텍처: ARM입니다.</span><span class="sxs-lookup"><span data-stu-id="bf0a9-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="bf0a9-114">해당 단계와 관련된 정보를 보려면 “[Microsoft Intune에서 Win32 앱의 추가, 할당 및 모니터링](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)” 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="bf0a9-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="bf0a9-115">Win32 앱을 포함하여 Windows에서 응용 프로그램 배포 문제 해결에 대한 자세한 내용은 다음 문서에서 검토 가능</span><span class="sxs-lookup"><span data-stu-id="bf0a9-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="bf0a9-116">앱 설치 문제 해결</span><span class="sxs-lookup"><span data-stu-id="bf0a9-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="bf0a9-117">Win32 앱 문제 해결</span><span class="sxs-lookup"><span data-stu-id="bf0a9-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)