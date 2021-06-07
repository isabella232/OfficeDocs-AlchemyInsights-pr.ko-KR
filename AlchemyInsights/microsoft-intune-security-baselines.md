---
title: 보안 Microsoft Intune 사용하여 Windows 10 구성
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783229"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="0145d-102">보안 Microsoft Intune 사용하여 Windows 10 구성</span><span class="sxs-lookup"><span data-stu-id="0145d-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="0145d-103">Intune 보안 기준은 사용자와 장치를 보호하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0145d-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="0145d-104">보안 기준은 Windows 팀에서 권장하는 알려진 설정 및 기본값 그룹을 적용하는 데 사용되는 미리 구성된 그룹에 대한 기본 설정입니다.</span><span class="sxs-lookup"><span data-stu-id="0145d-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="0145d-105">Intune에서 보안 기준 프로필을 만들어 여러 장치 구성 프로필로 구성된 서식 파일을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="0145d-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="0145d-106">사용자 또는 장치 그룹에 보안 기준을 배포하면 해당 설정이 사용자 또는 장치 그룹 이상에서 실행되는 Windows 10 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="0145d-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="0145d-107">예를 들어 Microsoft MDM(모바일 장치 관리) 보안 기준은 이동식 BitLocker 사용할 수 있는 보안 기준을 자동으로 설정하고, 디바이스 잠금을 해제하는 데 암호가 필요하며, 기본 인증을 사용하지 않도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="0145d-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="0145d-108">환경에서 기본값이 작동하지 않는 경우 필요한 설정을 적용하기 위해 기준을 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0145d-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="0145d-109">보안 기준은 Microsoft 365에서 엔드투엔드 보안 워크플로를 설정하는 데도 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0145d-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="0145d-110">보안 기준에는 보안에 영향을 주는 설정에 대한 모범 사례와 권장 사항이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0145d-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="0145d-111">그룹 정책에 대한 기준을 만드는 Windows 보안 팀과 Intune 파트너가 있으므로 이러한 권장 사항은 견고한 지침과 광범위한 환경을 기반으로 합니다.</span><span class="sxs-lookup"><span data-stu-id="0145d-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="0145d-112">Intune을 새로 사용하며 시작할 위치를 알 수 없는 경우 보안 기준을 사용하면 보안 프로필을 빠르게 만들고 배포할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0145d-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="0145d-113">현재 그룹 정책을 사용하는 경우 관리 목적으로 Intune으로 마이그레이션하는 것이 Intune에 기본 제공되어 최신 관리 기능을 포함하기 때문에 보안 기준을 훨씬 더 쉽게 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0145d-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="0145d-114">자세한 내용은 보안 [기준 Windows 모바일](/windows/security/threat-protection/windows-security-baselines) 장치 관리를 [참조하세요.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="0145d-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

