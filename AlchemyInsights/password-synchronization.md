---
title: 암호 동기화
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449142"
---
# <a name="password-synchronization"></a><span data-ttu-id="c36e3-102">암호 동기화</span><span class="sxs-lookup"><span data-stu-id="c36e3-102">Password synchronization</span></span>

<span data-ttu-id="c36e3-103">**암호 해시 동기화가 작동하지 않습니다.**</span><span class="sxs-lookup"><span data-stu-id="c36e3-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="c36e3-104">암호 해시 동기화가 작동하지 않을 때 고객에게 발생하는 몇 가지 일반적인 문제는 같습니다.</span><span class="sxs-lookup"><span data-stu-id="c36e3-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="c36e3-105">Azure AD Connect에서 사내 Active Directory와 통신하는 데 사용하는  Active Directory 계정에는 암호 동기화에 필요한 모든 복제 디렉터리 변경 및 복제 디렉터리 변경 권한이 부여되지 않습니다. Active Directory 계정에 이러한 사용 권한을 부여하여 이 문제를 해결해야 합니다. </span><span class="sxs-lookup"><span data-stu-id="c36e3-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="c36e3-106">암호 해시 동기화는 관리자가 사용자 Sign-In 메서드를 암호 동기화에서 Azure AD Connect 마법사의 **AD FS와의** 페더링과 같은 다른 옵션으로 변경한  후에 사용하지 않도록 설정됩니다. Azure AD Connect 마법사에서 암호 해시 동기화 기능을 다시 사용하도록 설정하면 이 문제를 해결할 수 있습니다. </span><span class="sxs-lookup"><span data-stu-id="c36e3-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="c36e3-107">프레미스 Active Directory의 연결 문제입니다.</span><span class="sxs-lookup"><span data-stu-id="c36e3-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="c36e3-108">예를 들어 일부 도메인 컨트롤러는 Azure AD Connect에서 [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) 액세스할 수 없는 경우 또는 필요한 포트가 방화벽에 의해 차단됩니다. Azure AD Connect 서버와 On-premises Active Directory 간의 연결이 올바르게 작동하는지 확인하여 이 문제를 해결해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c36e3-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="c36e3-109">Azure AD Connect 서버가 현재 준비 모드에 있습니다. 이 경우 서버가 암호 해시를 사용할 수 없습니다. 문제를 해결하기 위해 [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)동기화를 사용하여 암호 동기화 문제 해결 - 암호 동기화 없음 섹션에 설명된 단계를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="c36e3-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="c36e3-110">**일부 사용자에 대해 암호 해시 동기화가 작동하지 않습니다.**</span><span class="sxs-lookup"><span data-stu-id="c36e3-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="c36e3-111">사용자에 대해 암호 해시가 동기화되지 않는 경우  Azure AD Connect에서 문제 해결 작업을 사용하여 문제를 조사하고 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="c36e3-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="c36e3-112">다음 작업을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="c36e3-112">Perform the following tasks:</span></span>

    <span data-ttu-id="c36e3-113">a.</span><span class="sxs-lookup"><span data-stu-id="c36e3-113">a.</span></span> [<span data-ttu-id="c36e3-114">마법사에서 문제 해결 작업 실행</span><span class="sxs-lookup"><span data-stu-id="c36e3-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="c36e3-115">b.</span><span class="sxs-lookup"><span data-stu-id="c36e3-115">b.</span></span> [<span data-ttu-id="c36e3-116">문제 해결 cmdlet을 사용하여 특정 사용에 대한 암호 해시 동기화 문제 조사</span><span class="sxs-lookup"><span data-stu-id="c36e3-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="c36e3-117">사용자에 대해 사용할 수 있는 On-premises Active Directory User 개체는 다음 로그온 시 암호를 **변경해야** 합니다.</span><span class="sxs-lookup"><span data-stu-id="c36e3-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="c36e3-118">이 옵션을 사용하도록 설정하면 사용자에게 임시 암호가 할당되어 다음 로그온 시 암호를 변경하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="c36e3-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="c36e3-119">Azure AD Connect는 임시 암호를 Azure AD와 동기화하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c36e3-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="c36e3-120">위의 문제를 해결하기 위해 다음 작업 중 하나를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="c36e3-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="c36e3-121">사용자에게 프레미스 응용 프로그램(예: Windows 데스크톱)에 로그인하여 암호를 변경하도록 요청합니다.</span><span class="sxs-lookup"><span data-stu-id="c36e3-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="c36e3-122">새 암호가 Azure AD와 동기화됩니다.</span><span class="sxs-lookup"><span data-stu-id="c36e3-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="c36e3-123">관리자가 다음 로그온할 때 암호를 변경해야 합니다. 옵션을 사용하도록 설정하지 않고 사용자의 암호를 업데이트하도록 합니다. **및** 새 암호를 사용자와 공유합니다.</span><span class="sxs-lookup"><span data-stu-id="c36e3-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="c36e3-124">개체 동기화 또는 암호 동기화를  위해 On-premises Active Directory User 개체가 올바르게 구성되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c36e3-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="c36e3-125">이 문제를 해결하기 위해 Azure AD Connect 동기화를 사용하여 암호 해시 동기화 문제 [해결에 설명된 단계를 따릅니다.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="c36e3-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







