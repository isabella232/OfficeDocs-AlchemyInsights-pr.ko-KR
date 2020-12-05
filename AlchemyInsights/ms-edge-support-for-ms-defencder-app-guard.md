---
title: Microsoft Defender Application Guard에 대한 Microsoft Edge의 지원
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576547"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="be018-102">Microsoft Defender Application Guard에 대한 Microsoft Edge의 지원</span><span class="sxs-lookup"><span data-stu-id="be018-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="be018-103">Windows 10 및 Microsoft Edge용으로 설계된 Application Guard는 사용자가 호스트 운영 체제와 분리된 격리된 Hyper-V 사용 컨테이너 내에서 불안정한 사이트를 탐색할 수 있도록 하는 하드웨어 격리 방식을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="be018-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="be018-104">엔터프라이즈 관리자는 신뢰할 수 있는 웹 사이트, 클라우드 리소스 및 내부 네트워크 목록을 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="be018-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="be018-105">사용자가 목록에 없는 사이트를 방문하면 Microsoft Edge가 컨테이너에서 사이트를 웁니다.</span><span class="sxs-lookup"><span data-stu-id="be018-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="be018-106">즉, 사이트가 악의적인 것으로 나타날 경우 호스트 PC는 보호된 상태로 유지되어 공격자가 엔터프라이즈 데이터에 액세스하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="be018-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="be018-107">컨테이너에 확장을 설치하는 것은 Microsoft Edge 버전 81에서 지원하며 정책을 통해 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="be018-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="be018-108">ExtensionInstallForcelist 정책에서 사용되는 updateURL 주소는 Application Guard에서 사용하는 네트워크 고리 정책에서 중립 리소스로 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="be018-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="be018-109">자세한 내용은 [Microsoft Defender Application Guard에](https://go.microsoft.com/fwlink/?linkid=2134229)대한 Microsoft Edge 지원을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="be018-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
