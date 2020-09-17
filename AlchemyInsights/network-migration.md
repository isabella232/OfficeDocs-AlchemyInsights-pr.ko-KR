---
title: 네트워크 마이그레이션
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "716"
- "6000002"
ms.assetid: b5ab885c-3803-4cc8-adab-94848e226ffb
ms.openlocfilehash: 6f026f932bb35d12d32ce7eddf49e49a44db7f31
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799570"
---
# <a name="network-migration"></a><span data-ttu-id="6a6b0-102">네트워크 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="6a6b0-102">Network Migration</span></span>

<span data-ttu-id="6a6b0-103">O365 테 넌 트가 1 테 넌 트의 여러 Yammer 네트워크 (많은 네트워크 구성)에 연결 되어 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6a6b0-103">Your O365 tenant is possibly associated with multiple Yammer networks in a 1 tenant : Many networks configuration.</span></span> <span data-ttu-id="6a6b0-104">2018 년 10 월 16 일부터 Yammer는 한 테 넌 트에서 연결 된 다중 Yammer 네트워크를 더 이상 지원 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6a6b0-104">Starting October 16, 2018, Yammer will no longer support multiple Yammer networks associated with one tenant.</span></span> <span data-ttu-id="6a6b0-105">네트워크 마이그레이션을 수행 하 여 기본 1:1 구성에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6a6b0-105">You can perform a Network Migration to get to a preferred 1:1 configuration.</span></span>
  
- <span data-ttu-id="6a6b0-106">테 넌 트와 연결 된 네트워크 목록을 보려면 전역 관리자로 Yammer에 로그인 하 고 **네트워크 관리자로**이동한 다음 **네트워크 마이그레이션을**사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="6a6b0-106">To view a list of the networks associated with your tenant, log in to Yammer as an Global Administrator and browse to **Network Admin**, then **Network Migration**.</span></span> <span data-ttu-id="6a6b0-107">**다음**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="6a6b0-107">Choose **Next**.</span></span>

- <span data-ttu-id="6a6b0-108">2 단계 중에 여러 개의 네트워크가 표시 되는 경우에는 사용자의 O365 테 넌 트와 연결 된 Yammer 네트워크가 여러 개 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6a6b0-108">If you see multiple networks listed on Step 2 of 3, then you have multiple Yammer networks associated with your O365 tenant.</span></span>

- <span data-ttu-id="6a6b0-109">1:1 구성에 대 한 구성을 수정 하려면 네트워크 마이그레이션 도구를 계속 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="6a6b0-109">To correct your configuration to a 1:1 configuration, continue using the Network Migration tool.</span></span>

- <span data-ttu-id="6a6b0-110">네트워크 마이그레이션에 대 한 자세한 내용은 [네트워크 마이그레이션: 여러 Yammer 네트워크 통합](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="6a6b0-110">For more information on Network Migration please see [Network migration: Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

<span data-ttu-id="6a6b0-111">참고 사항:</span><span class="sxs-lookup"><span data-stu-id="6a6b0-111">Please Note:</span></span>
  
- <span data-ttu-id="6a6b0-112">**네트워크 마이그레이션은 활성 및 보류 중인 사용자만 마이그레이션합니다.**</span><span class="sxs-lookup"><span data-stu-id="6a6b0-112">**A network migration migrates only the active and pending users.**</span></span> <span data-ttu-id="6a6b0-113">활성 사용자와 함께 이름 및 프로필 그림과 같은 사용자 정보도 마이그레이션됩니다.</span><span class="sxs-lookup"><span data-stu-id="6a6b0-113">Along with the active users, the users' information, such as name and profile picture, is also migrated.</span></span> <span data-ttu-id="6a6b0-114">그룹을 포함 하는 모든 네트워크 콘텐츠는 마이그레이션되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6a6b0-114">Any network content, including groups, is not migrated.</span></span>

- <span data-ttu-id="6a6b0-115">**네트워크 마이그레이션을 되돌릴 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="6a6b0-115">**Network migration can't be reversed.**</span></span> <span data-ttu-id="6a6b0-116">마이그레이션 후에는 자회사 네트워크 및 해당 콘텐츠에 액세스할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="6a6b0-116">You will not be able to access your subsidiary network and its content after migration.</span></span> <span data-ttu-id="6a6b0-117">따라서 마이그레이션을 고려 하기 전에 신중한 계획을 세워야 합니다.</span><span class="sxs-lookup"><span data-stu-id="6a6b0-117">So before you consider a migration, you want to plan carefully.</span></span>
