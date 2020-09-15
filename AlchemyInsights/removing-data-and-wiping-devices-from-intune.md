---
title: Intune에서 데이터 삭제하고 장치 초기화
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
- "1279"
- "6700008"
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701289"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="dc622-102">Intune에서 데이터 삭제하고 장치 초기화</span><span class="sxs-lookup"><span data-stu-id="dc622-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="dc622-103">Intune에서 회사 데이터를 삭제하거나 공장 초기화를 실행하고 장치를 기본 설정으로 되돌리기 위해 장치 사용 중지 및 장치 초기화 원격 작업을 사용 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dc622-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="dc622-104">Microsoft 365 장치 관리에 로그인하고 **장치** > **모든 장치**로 이동하세요.</span><span class="sxs-lookup"><span data-stu-id="dc622-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="dc622-105">초기화 할 장치를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="dc622-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="dc622-106">원하는 원격 초기화 유형을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="dc622-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="dc622-107">사용 중지는 조직 정보만 삭제하고 전체 초기화는 장치를 공장 설정으로 복원합니다.</span><span class="sxs-lookup"><span data-stu-id="dc622-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="dc622-108">**예**를 선택하여 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="dc622-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="dc622-109">장치가 삭제될 때까지 장치 활동 상태는 사용 중지 보류 중으로 보여집니다.</span><span class="sxs-lookup"><span data-stu-id="dc622-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="dc622-110">작업이 완료되면 관리되는 장치 목록에서 모바일 장치를 볼 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="dc622-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="dc622-111">**참고** Azure AD에 연결 된 장치에서는 회사 데이터를 제거할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="dc622-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="dc622-112">유지되는 항목 및 삭제 되는 항목을 포함하여 사용 중지 및 초기화 작업 영향에 대한 자세한 내용은 [초기화, 사용 중지 혹은 수동으로 장치 등록 삭제하기를 사용하여 장치 삭제](https://docs.microsoft.com/intune/devices-wipe)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="dc622-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="dc622-113">MacOS 장치에서 모든 데이터를 지우려면 [MacOS 장치에서 모든 데이터 지우기](https://docs.microsoft.com/intune/device-erase)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="dc622-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>