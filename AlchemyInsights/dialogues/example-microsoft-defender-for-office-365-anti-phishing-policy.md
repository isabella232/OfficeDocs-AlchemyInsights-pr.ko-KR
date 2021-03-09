---
title: 예제 Microsoft Defender for Office 365 피싱 방지 정책
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552420"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="df449-102">예제 Microsoft Defender for Office 365 피싱 방지 정책</span><span class="sxs-lookup"><span data-stu-id="df449-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="df449-103">이러한 설정을 사용하면 Domain 및 *CEO라는 정책을 사용할 수 있습니다.*</span><span class="sxs-lookup"><span data-stu-id="df449-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="df449-104">이 정책은 가장으로부터 사용자 및 도메인 보호를 모두 제공한 다음 도메인 내의 사용자가 받은 모든 전자 메일에 정책을 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="df449-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="df449-105">먼저 다음 정보를 추가하여 정책을 생성합니다.</span><span class="sxs-lookup"><span data-stu-id="df449-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="df449-106">**이름:** 도메인 및 CEO **설명:** CEO와 도메인이 가장되지 않는지 확인</span><span class="sxs-lookup"><span data-stu-id="df449-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="df449-107">**적용 대상:** 받는 **사람 도메인이 입니다.를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="df449-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="df449-108">다음 중 어느  **것에서** 선택을 선택하고 도메인을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="df449-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="df449-109">**+ 추가** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="df449-109">Select **+ Add**.</span></span> <span data-ttu-id="df449-110">목록에서 도메인 이름 옆에 있는 확인란을 선택하고 *(예:* contoso.com ) 추가를 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="df449-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="df449-111">**완료** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="df449-111">Select **Done**.</span></span>
- <span data-ttu-id="df449-112">정책을 만든 후 다음 옵션을 사용하여 정책을 미세 조정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="df449-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="df449-113">**보호할 사용자를 추가합니다.** 이 예에서는 최소한 CEO의 전자 메일 주소를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="df449-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="df449-114">**보호할 도메인 추가:** CEO 사무실을 포함하는 조직 도메인을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="df449-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="df449-115">**작업 선택**: **가장된** 사용자가 전자 메일을 보낸 경우 메시지를 다른 전자 메일 주소로 리디렉션을 선택한 다음 보안 관리자의 전자 메일 주소(예: *securityadmin@contoso.com)를 입력합니다.*</span><span class="sxs-lookup"><span data-stu-id="df449-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="df449-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span><span class="sxs-lookup"><span data-stu-id="df449-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="df449-117">**사서함 인텔리전스:** 기본적으로 이 옵션은 새 피싱 방지 정책을 만들 때 선택됩니다.</span><span class="sxs-lookup"><span data-stu-id="df449-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="df449-118">최상의 결과를 위해 해당 설정을 **켜짐** 에 둡니다.</span><span class="sxs-lookup"><span data-stu-id="df449-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="df449-119">**신뢰할 수 있는 보낸 사람 및 도메인을 추가합니다.** 이 예제에서는 모든 오버라이드를 정의하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="df449-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="df449-120">설정을 검토한 후 이 정책  만들기 또는 **저장을** 적절하게 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="df449-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="df449-121">자세한 내용은 [Microsoft 365의](https://go.microsoft.com/fwlink/?linkid=2092235)피싱 방지 정책을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="df449-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
