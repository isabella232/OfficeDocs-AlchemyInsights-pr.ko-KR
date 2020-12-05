---
title: Windows에서 Microsoft Edge 정책 설정 구성
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
- "9003845"
- "6894"
ms.openlocfilehash: 7f626152c3833638436dfe05e8dcd13fc86ef594
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576476"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="abdea-102">Windows에서 Microsoft Edge 정책 설정 구성</span><span class="sxs-lookup"><span data-stu-id="abdea-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="abdea-103">Microsoft Edge에 대한 정책 설정 및 관리되는 업데이트를 구성하려면 GOS(그룹 정책 개체)를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="abdea-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="abdea-104">레지스트리를 통해 정책을 프로비전할 수도 있습니다. 이는 (1) Microsoft Active Directory 도메인에 가입된 Windows 장치 및 (2) Microsoft Intune에서 장치 관리를 위해 등록된 Windows 10 Pro 및 엔터프라이즈 인스턴스에 적합합니다.</span><span class="sxs-lookup"><span data-stu-id="abdea-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="abdea-105">GOS를 사용하여 Microsoft Edge를 구성하기 위해 다음을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="abdea-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="abdea-106">Active Directory 도메인의 그룹 정책 중앙 저장소 또는 개별 컴퓨터의 정책 정의 템플릿 폴더에 Microsoft Edge에 대한 규칙 및 설정을 추가하는 모든 관리 템플릿을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="abdea-106">To the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="abdea-107">설정할 특정 정책을 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="abdea-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="abdea-108">자세한 내용은 Windows에서 Microsoft Edge 정책 설정 [구성을 참조하세요.](https://go.microsoft.com/fwlink/?linkid=2135024)</span><span class="sxs-lookup"><span data-stu-id="abdea-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
