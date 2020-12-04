---
title: Microsoft Intune 보안 기준을 사용하여 Windows 10 장치 구성
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571896"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="c62cc-102">Microsoft Intune 보안 기준을 사용하여 Windows 10 장치 구성</span><span class="sxs-lookup"><span data-stu-id="c62cc-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="c62cc-103">Intune 보안 기준은 사용자 및 장치를 보호하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c62cc-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="c62cc-104">보안 기준은 관련 보안 팀에서 권장하는 알려진 설정 그룹 및 기본값을 적용하는 데 사용되는 Windows 설정의 미리 구성된 그룹입니다.</span><span class="sxs-lookup"><span data-stu-id="c62cc-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="c62cc-105">Intune에서 보안 기준 프로필을 만들면 여러 장치 구성 프로필로 구성된 템플릿을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c62cc-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="c62cc-106">사용자 또는 장치 그룹에 보안 기준을 배포하면 설정이 Windows 10 이상에서 실행되는 장치에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="c62cc-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="c62cc-107">예를 들어 MDM 보안 기준(1)은 이동식 드라이브에 대해 BitLocker를 활성화하고, (2)장치의 잠금을 해제하는 데 암호가 필요하며, (3) 기본 인증을 사용하지 않도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="c62cc-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="c62cc-108">환경에서 기본값이 작동하지 않는 경우 필요한 설정을 적용하기 위해 기준을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="c62cc-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="c62cc-109">보안 기준은 Microsoft 365에서 종단식 보안 워크플로를 설정하는 데에도 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c62cc-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="c62cc-110">이 경우의 몇 가지 이점은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="c62cc-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="c62cc-111">보안 기준에는 보안에 영향을 주는 설정에 대한 모범 사례 및 권장 사항이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c62cc-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="c62cc-112">그룹 정책에 대한 기준을 만드는 Windows 보안 팀과 Intune 파트너가 있기 때문에 이러한 권장 사항은 견고한 지침과 광범위한 환경을 기반으로 합니다.</span><span class="sxs-lookup"><span data-stu-id="c62cc-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="c62cc-113">Intune을 새로 사용하며 시작할 위치를 알 수 없는 경우 보안 기준을 통해 보안 프로필을 빠르게 만들고 배포할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c62cc-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="c62cc-114">현재 그룹 정책을 사용하는 경우 관리 목적으로 Intune으로 마이그레이션하는 것이 훨씬 더 쉬워집니다. 이러한 정책은 Intune에 기본 제공되어 관리에 대한 최신 기능을 포함하기 때문에 보안 기준을 훨씬 더 쉽게 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c62cc-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="c62cc-115">자세한 내용은 [Windows 보안](https://go.microsoft.com/fwlink/?linkid=2141503) 기준 및 모바일 장치 [관리를 참조하세요.](https://go.microsoft.com/fwlink/?linkid=2141701)</span><span class="sxs-lookup"><span data-stu-id="c62cc-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>