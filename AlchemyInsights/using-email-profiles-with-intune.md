---
title: Intune에서 전자 메일 프로필 사용
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505215"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="3d7d4-102">Intune에서 전자 메일 프로필 사용</span><span class="sxs-lookup"><span data-stu-id="3d7d4-102">Using email profiles with Intune</span></span>

<span data-ttu-id="3d7d4-103">Intune을 사용하여 기본(기본 제공) 전자 메일 클라이언트의 전자 메일 프로필을 만들고 여러 장치 플랫폼에 배포할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3d7d4-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="3d7d4-104">기존 프로필이 처리되는 방식과 전자 메일 프로필을 제거하는 방법을 비롯하여 전자 메일 프로필과 관련된 일부 제한 사항에 대한 자세한 내용은 [Intune을 사용하여 장치에 전자 메일 설정 추가](https://docs.microsoft.com/intune/email-settings-configure)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="3d7d4-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="3d7d4-105">각 장치 플랫폼의 전자 메일 프로필을 만드는 방법에 대한 자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="3d7d4-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="3d7d4-106">Android 장치 설정을 사용하여 Intune에서 전자 메일, 인증 및 동기화 구성</span><span class="sxs-lookup"><span data-stu-id="3d7d4-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="3d7d4-107">Microsoft Intune에서 iOS 및 iPadOS 장치의 전자 메일 설정 추가</span><span class="sxs-lookup"><span data-stu-id="3d7d4-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="3d7d4-108">Windows Phone 8.1을 실행하는 장치에 대한 Microsoft Intune의 전자 메일 프로필 설정</span><span class="sxs-lookup"><span data-stu-id="3d7d4-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="3d7d4-109">Microsoft Intune에서 Windows 10을 실행하는 장치의 전자 메일 프로필 설정</span><span class="sxs-lookup"><span data-stu-id="3d7d4-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="3d7d4-110">**일반적인 동기화 문제**</span><span class="sxs-lookup"><span data-stu-id="3d7d4-110">**Common syncing issue**</span></span>

<span data-ttu-id="3d7d4-111">**Android 전자 메일 프로필의 KNOX를 사용하면 사용자 연락처, 일정 및 작업이 사용자 장치와 동기화되지 않습니다.**</span><span class="sxs-lookup"><span data-stu-id="3d7d4-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="3d7d4-112">Android KNOX 전자 메일 프로필을 사용하면 관리자가 각 항목을 활성화하여 장치와 동기화할 콘텐츠 형식을 결정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3d7d4-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="3d7d4-113">콘텐츠 형식에 대한 설정이 **구성되지 않음**(기본값)으로 설정된 경우, 해당 콘텐츠 형식은 자동으로 동기화되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="3d7d4-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="3d7d4-114">사용자가 수동으로 장치에서 원하는 콘텐츠 형식을 직접 활성화할 수 있지만, Intune 정책 설정이 해당 구성을 덮어쓰고 해당 콘텐츠 형식에 대한 동기화가 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="3d7d4-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

