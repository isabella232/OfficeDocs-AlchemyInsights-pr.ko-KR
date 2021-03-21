---
title: SCP(서비스 연결 지점 구성)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898065"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="07eaf-102">SCP(서비스 연결 지점 구성)</span><span class="sxs-lookup"><span data-stu-id="07eaf-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="07eaf-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="07eaf-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="07eaf-104">**이유**: SCP 개체를 읽고 Azure AD 테넌트 정보를 얻을 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="07eaf-105">**해결**: [서비스 연결 지점 구성](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join) 섹션을 참고하세요.</span><span class="sxs-lookup"><span data-stu-id="07eaf-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="07eaf-106">**실행 계획**</span><span class="sxs-lookup"><span data-stu-id="07eaf-106">**Action plan**</span></span>

- <span data-ttu-id="07eaf-107">장치가 제어된 유효성 검사에 대한 GPO를 받았는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="07eaf-108">GPO에서 레지스트리 키를 만들었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="07eaf-109">디렉터리 ID와 onmicrosoft 도메인으로 키 2개가 만들어졌다는 것을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="07eaf-110">**SCP에 대한 클라이언트 레지스트리 설정 구성**</span><span class="sxs-lookup"><span data-stu-id="07eaf-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="07eaf-111">다음 예제를 사용하여 GPO(그룹 정책 개체)를 만들어 장치의 레지스트리에서 SCP 항목을 구성하는 레지스트리 설정을 배포합니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="07eaf-112">그룹 정책 관리 콘솔을 열고 도메인에 새 GPO를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="07eaf-113">새로 만든 GPO의 이름(예: ClientSideSCP)을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="07eaf-114">GPO를 편집하고 다음 경로를 찾습니다. **컴퓨터 구성 > 기본 설정 > Windows 설정 > 레지스트리**.</span><span class="sxs-lookup"><span data-stu-id="07eaf-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="07eaf-115">**레지스트리** 에 오른쪽 클릭하고 **신규 > 레지스트리 항목** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="07eaf-116">**일반** 탭에서 다음을 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="07eaf-117">**작업**: 업데이트</span><span class="sxs-lookup"><span data-stu-id="07eaf-117">**Action**: Update</span></span>
    
- <span data-ttu-id="07eaf-118">**Hive**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="07eaf-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="07eaf-119">**키 경로**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="07eaf-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="07eaf-120">**값 이름**: TenantId</span><span class="sxs-lookup"><span data-stu-id="07eaf-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="07eaf-121">**값 형식**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="07eaf-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="07eaf-122">**값 데이터**: Azure AD 인스턴스의 GUID 또는 디렉터리 ID(이 값은 **Azure Portal > Azure Active Directory > 속성 > 디렉터리 ID**)에서 찾을 수 있음)</span><span class="sxs-lookup"><span data-stu-id="07eaf-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="07eaf-123">**확인** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="07eaf-124">**레지스트리** 에 오른쪽 클릭하고 **신규 > 레지스트리 항목** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="07eaf-125">**일반** 탭에서 다음을 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="07eaf-126">**작업**: 업데이트</span><span class="sxs-lookup"><span data-stu-id="07eaf-126">**Action**: Update</span></span>
    
- <span data-ttu-id="07eaf-127">**Hive**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="07eaf-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="07eaf-128">**키 경로**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="07eaf-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="07eaf-129">**값 이름**: TenantName</span><span class="sxs-lookup"><span data-stu-id="07eaf-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="07eaf-130">**값 형식**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="07eaf-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="07eaf-131">**값 데이터**: AD FS와 같은 페더레이션된 환경을 사용하는 경우 확인된 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="07eaf-132">관리되는 환경을 사용하는 경우 확인된 도메인 이름 또는 onmicrosoft.com 도메인 이름(예: contoso.onmicrosoft)입니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="07eaf-133">**확인** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-133">Click **OK**.</span></span>

7. <span data-ttu-id="07eaf-134">새로 만든 GPO의 편집기를 닫습니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="07eaf-135">제어된 출시 인구에 속하는 도메인에 가입된 컴퓨터를 포함하여 원하는 OU에 새로 만든 GPO를 연결합니다.</span><span class="sxs-lookup"><span data-stu-id="07eaf-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="07eaf-136">자세한 내용은  [하이브리드 Azure AD 제어 유효성 검사 참가 - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) 및  [하이브리드 Azure Active Directory에 가입된 장치 문제해결 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)을 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="07eaf-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









