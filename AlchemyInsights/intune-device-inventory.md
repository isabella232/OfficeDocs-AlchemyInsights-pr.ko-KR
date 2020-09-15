---
title: Intune 장치 인벤토리
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667884"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="c828a-102">Intune 장치 인벤토리</span><span class="sxs-lookup"><span data-stu-id="c828a-102">Intune Device Inventory</span></span>

<span data-ttu-id="c828a-103">장치 블레이드에서는 장치 단위로 Intune에서 관리 중인 장치에 대한 관리자 인싸이트를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="c828a-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="c828a-104">하드웨어, 검색 된 응용 프로그램, 장치 준수 상태 및 장치 구성 상태 등을 포함한 정보가 보여집니다.</span><span class="sxs-lookup"><span data-stu-id="c828a-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="c828a-105">하드웨어 및 검색 된 응용 프로그램 인벤토리 데이터는 7일 주기로 수집됩니다.</span><span class="sxs-lookup"><span data-stu-id="c828a-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="c828a-106">보고되는 하드웨어의 응용 프로그램 및 특정 요소는 장치 운영 체제와 장치가 개인용인지 회사용인지 여부에 따라 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="c828a-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="c828a-107">자세한 내용은 [Intune에서 장치 자세히 보기](https://docs.microsoft.com/intune/device-inventory)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c828a-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="c828a-108">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="c828a-108">**FAQ**</span></span>

<span data-ttu-id="c828a-109">Q: Intune에 등록 된 Windows 장치에 존재하는 응용 프로그램에 전체 인벤터리 목록을 받고 있지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c828a-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="c828a-110">그 이유는 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="c828a-110">Why not?</span></span>

<span data-ttu-id="c828a-111">A:이 경우에는 회사 장치로 식별되는 Windows 10 PC 최신 앱만 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c828a-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="c828a-112">Intune이 이 장치에 설치 된 Win32 앱 정보를 수집 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c828a-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="c828a-113">Q: 모든 장치에서 전화 번호가 수집 되지 않는 이유는 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="c828a-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="c828a-114">A: 예를 들어, 사용자가 모바일 장치 인벤터리 보고서를 실행 할 때 Intune에서 회사 장치로 분류되는 전화의 전체 전화 번호는 식별되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c828a-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="c828a-115">나만의 장치 전화 번호는 항상 별표 (\*\*\*\*)로 부분적으로 마스킹 하고 마지막 네 자릿수만 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="c828a-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>