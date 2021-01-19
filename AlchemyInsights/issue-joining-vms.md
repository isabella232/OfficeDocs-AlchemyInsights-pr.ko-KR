---
title: VM 조인 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884584"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="044c6-102">VM 조인 문제</span><span class="sxs-lookup"><span data-stu-id="044c6-102">Issue joining VMs</span></span>

<span data-ttu-id="044c6-103">VM을 조인하는 동안 발생하는 문제를 해결하려면 다음 단계를 수행하세요.</span><span class="sxs-lookup"><span data-stu-id="044c6-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="044c6-104">**SAMAccountName** 형식 대신 **UPN** 형식(예: 'joeuser@contoso.com')을 사용하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="044c6-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="044c6-105">*시작 가이드* 에 설명된 단계에 따라 암호 동기화를 사용 가능으로 설정했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="044c6-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="044c6-106">영향을 받는 사용자 계정이 Azure AD 테넌트의 외부 계정이 아닌지 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="044c6-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="044c6-107">Azure AD Domain Services에는 이러한 사용자 계정에 대한 자격 증명이 없기 때문에 외부 사용자가 관리 도메인에 로그인할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="044c6-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="044c6-108">영향을 받는 사용자 계정이 클라우드 전용 사용자 계정인 경우 Azure AD Domain Services를 사용하도록 설정한 후 사용자가 암호를 변경했는지 확인하십시오.</span><span class="sxs-lookup"><span data-stu-id="044c6-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="044c6-109">이 단계에서는 Azure AD Domain Services를 생성하는 데 필요한 자격 증명 해시를 생성합니다.</span><span class="sxs-lookup"><span data-stu-id="044c6-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="044c6-110">영향을 받는 사용자 계정이 온-프레미스 디렉토리에서 동기화되는 경우 Azure AD Connect의 권장 릴리스가 전체 동기화를 수행하도록 구성되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="044c6-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="044c6-111">4단계를 확인한 후에도 문제가 지속되면 동기화 시스템에서 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="044c6-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="044c6-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="044c6-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>