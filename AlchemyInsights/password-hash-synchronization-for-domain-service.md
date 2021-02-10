---
title: 도메인 서비스에 대한 암호 해시 동기화
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162942"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="98e33-102">도메인 서비스에 대한 암호 해시 동기화</span><span class="sxs-lookup"><span data-stu-id="98e33-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="98e33-103">**Azure AD DS 인스턴스에 암호 해시 동기화를 사용하도록 설정하라는 메시지가 표시될 경우**</span><span class="sxs-lookup"><span data-stu-id="98e33-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="98e33-104">사용자가 온-프레미스 Azure AD DS(도메인 서비스) 환경에서 동기화하는 하이브리드 환경을 실행하는 시나리오가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="98e33-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="98e33-105">이 시나리오는 온-프레미스 AD DS에서 Azure AD 테넌트로 암호 해시 동기화가 있는 경우 발생됩니다.</span><span class="sxs-lookup"><span data-stu-id="98e33-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="98e33-106">**원인**</span><span class="sxs-lookup"><span data-stu-id="98e33-106">**Cause**</span></span>

<span data-ttu-id="98e33-107">Azure AD Connect는 기본적으로 Azure AD DS에 필요한 레거시 새 기술 LAN 관리자(NTLM) 및 Kerberos 암호 해시를 동기화하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="98e33-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="98e33-108">**해결 방법**</span><span class="sxs-lookup"><span data-stu-id="98e33-108">**Workaround**</span></span> 

<span data-ttu-id="98e33-109">NTLM 및 Kerberos 인증에 필요한 암호 해시를 동기화하려면 Azure AD Connect를 구성해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="98e33-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="98e33-110">Azure AD Connect가 구성된 후에는 온-프레미스 계정 만들기 또는 암호 변경 이벤트도 Azure AD에 레거시 암호 해시를 동기화합니다.</span><span class="sxs-lookup"><span data-stu-id="98e33-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="98e33-111">Azure AD DS 하이브리드 환경에서 암호 동기화를 설정하는 방법에 대한 지침은 [여기](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="98e33-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>