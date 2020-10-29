---
title: Intune Exchange 온-프레미스 커넥터
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791522"
---
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="b845d-102">Intune Exchange 온-프레미스 커넥터</span><span class="sxs-lookup"><span data-stu-id="b845d-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="b845d-103">Intune과 온-프레미스에 호스트 되는 Exchange 사이에 커넥터를 설정 하는 방법에 대 한 자세한 내용은 다음 설명서를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="b845d-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="b845d-104">Microsoft Intune Azure에서 Intune 온-프레미스 Exchange 커넥터 설정</span><span class="sxs-lookup"><span data-stu-id="b845d-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="b845d-105">**자주 묻는 질문(FAQ):**</span><span class="sxs-lookup"><span data-stu-id="b845d-105">**FAQ:**</span></span>

<span data-ttu-id="b845d-106">Q: Exchange connector를 설정 하려고 할 때 "Exchange Connector 버전이 지원 되지 않습니다."와 같은 오류가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b845d-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="b845d-107">원인은 무엇 인가요?</span><span class="sxs-lookup"><span data-stu-id="b845d-107">What could be the cause?</span></span>

<span data-ttu-id="b845d-108">A: 사용 중인 계정에 적절 한 라이선스가 부여 된 경우-활성 Intune 라이선스가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b845d-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="b845d-109">Q: 여러 Exchange 커넥터를 사용할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="b845d-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="b845d-110">A: exchange 조직 당 Intune 테 넌 트 당 하나의 Exchange 커넥터만 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b845d-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="b845d-111">커넥터는 다중 서버 exchange 조직의 한 서버에만 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b845d-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="b845d-112">또한 같은 테 넌 트에서 구성 된 Exchange 온-프레미스 및 Exchange Online 모두에 대해 커넥터를 구성할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b845d-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="b845d-113">Q: 커넥터가 CAS 배열을 Exchange 연결로 사용할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="b845d-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="b845d-114">A: CAS 배열을 지정 하는 것은 커넥터 설정에서 지원 되지 않는 구성입니다.</span><span class="sxs-lookup"><span data-stu-id="b845d-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="b845d-115">단일 서버만 지정 해야 하며, 다음 위치에서 찾을 수 있는 커넥터 구성 파일에 하드 코드 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b845d-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="b845d-116">온-프레미스 Exchange 커넥터에 data\microsoft\microsoft Intune 프로그램 \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="b845d-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="b845d-117">다음 항목을 찾아 ```<ExchangeWebServiceURL />``` URL을 exchange 서버로 바꿉니다.</span><span class="sxs-lookup"><span data-stu-id="b845d-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="b845d-118">**예에서**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="b845d-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="b845d-119">추가 문제 해결 방법은 다음 설명서를 참조 하세요. [Intune 온-프레미스 Exchange Connector 문제 해결](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="b845d-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="b845d-120">**Exchange 커넥터에 대해 자세한 정보 표시 로깅 사용**</span><span class="sxs-lookup"><span data-stu-id="b845d-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="b845d-121">Exchange Connector 추적 구성 파일을 편집용으로 엽니다.</span><span class="sxs-lookup"><span data-stu-id="b845d-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="b845d-122">파일 은%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b845d-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="b845d-123">**예에서**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="b845d-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="b845d-124">다음 키를 사용 하 여 TraceSourceLine를 찾습니다. OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="b845d-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="b845d-125">정보 ActivityTracing (기본값)에서 SourceLevel node 값을 자세한 ActivityTracing로 변경 합니다.</span><span class="sxs-lookup"><span data-stu-id="b845d-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="b845d-126">**예제:**</span><span class="sxs-lookup"><span data-stu-id="b845d-126">**Example:**</span></span>
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. <span data-ttu-id="b845d-127">Microsoft Intune Exchange 서비스 다시 시작</span><span class="sxs-lookup"><span data-stu-id="b845d-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="b845d-128">Intune 포털에서 전체 동기화-완료 된 다음 XML을 다시 "Information ActivityTracing"로 변경 하 고 Microsoft Intune Exchange 서비스를 다시 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="b845d-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="b845d-129">로그 위치는 다음과 같습니다. `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="b845d-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>