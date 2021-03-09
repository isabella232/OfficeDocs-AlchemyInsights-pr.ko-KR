---
title: 네트워크 메시지 ID를 제공하여 전자 메일 메시지 제출
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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552356"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="b0cfd-102">네트워크 메시지 ID를 제공하여 전자 메일 메시지 제출</span><span class="sxs-lookup"><span data-stu-id="b0cfd-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="b0cfd-103">새 제출 **플라이아웃에서** 전자 **메일** 및 네트워크 메시지 **ID 를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="b0cfd-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="b0cfd-104">다음 단계에 따라 Outlook에서 전자 메일 메시지의 메시지 ID를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0cfd-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="b0cfd-105">전자 메일 메시지를 두 번 클릭하여 열립니다.</span><span class="sxs-lookup"><span data-stu-id="b0cfd-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="b0cfd-106">파일 **속성**  >  **을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="b0cfd-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="b0cfd-107">메모장이나 빈 Word 문서를 연 다음 인터넷 헤더 상자에 있는 콘텐츠를 복사하여 열려 있는 문서에 붙여넣어 보다 쉽게 가시성을 확보할 수 있습니다. </span><span class="sxs-lookup"><span data-stu-id="b0cfd-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="b0cfd-108">**X-MS-Exchange-Organization-Network-Message-Id 필드를** 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="b0cfd-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="b0cfd-109">의 다음 값은 **제출에** 필요한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b0cfd-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="b0cfd-110">받는 **사람 아래에서** 이 전자 메일의 모든 받는 사람에 대한 정크 메일 폴더에 전자 메일이 전송된 경우 모두 **선택 을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="b0cfd-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="b0cfd-111">그렇지 않은 경우 문제를 보고한 사용자만 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b0cfd-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="b0cfd-112">제출 **이유 에서** 차단해야 를 선택하는 경우 메시지가 스팸, 피싱 또는 맬웨어로 차단된 것인지를 지정한 다음 제출을  **선택합니다.** </span><span class="sxs-lookup"><span data-stu-id="b0cfd-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="b0cfd-113">자세한 내용은 검색을 위해 의심되는 스팸, 피싱, URL 및 파일을 [Microsoft에 제출하는 방법을 참조합니다.](https://go.microsoft.com/fwlink/?linkid=2101479)</span><span class="sxs-lookup"><span data-stu-id="b0cfd-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
