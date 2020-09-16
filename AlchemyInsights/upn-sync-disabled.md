---
title: UPN 동기화 사용 안 함
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749520"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="4abd5-102">UPN 동기화 사용 안 함</span><span class="sxs-lookup"><span data-stu-id="4abd5-102">UPN sync disabled</span></span>

<span data-ttu-id="4abd5-103">2016 년 3 월 30 일 이전에 Azure AD에 동기화를 시작한 경우 다음 Azure AD PowerShell cmdlet을 실행 하 여 조직에 대해서만 UPN 소프트 일치를 사용 하도록 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="4abd5-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="4abd5-104">**MsolDirSyncFeature-EnableSoftMatchOnUpn 기능을 사용 하도록 설정 $True**</span><span class="sxs-lookup"><span data-stu-id="4abd5-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="4abd5-105">UPN soft match는 Azure AD에 대 한 동기화를 시작한 조직에 대해 자동으로 설정 되며, 2016 년 3 월 30 일 이후에 시작 됩니다.</span><span class="sxs-lookup"><span data-stu-id="4abd5-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="4abd5-106">UPN 및 기타 동기화 기능에 대해 소프트 일치를 사용 하도록 설정 하는 방법에 대 한 자세한 내용은 [AZURE AD Connect sync service 기능](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="4abd5-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

