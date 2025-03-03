---
title: Microsoft Defender for Endpoint SmartScreen URL reputation demonstrations
description: Demonstrates how Microsoft Defender SmartScreen identifies phishing and malware websites based on URL reputation.
search.appverid: met150
ms.service: defender-endpoint
ms.author: siosulli
author: siosulli
ms.localizationpriority: medium
manager: deniseb
audience: ITPro
ms.collection:
- m365-security
- tier2
- demo
ms.topic: article
ms.subservice: asr
ms.date: 01/15/2024
---

# URL reputation demonstrations

**Applies to:**

- [Microsoft Defender for Endpoint Plan 2](https://go.microsoft.com/fwlink/p/?linkid=2154037)
- [Microsoft Defender for Business](https://www.microsoft.com/security/business/endpoint-security/microsoft-defender-business)
- [Microsoft Defender for Endpoint Plan 1](https://go.microsoft.com/fwlink/p/?linkid=2154037)

Test how Microsoft Defender SmartScreen helps you identify phishing and malware websites based on URL reputation.
Scenario requirements and setup

- Windows 11 or Windows
- Windows Server 2022, Windows Server 2019, Windows Server 2016, Windows Server 2012 R2 and Windows Server 2008 R2 SP1.
- Microsoft Edge browser required
- For more information, see [Microsoft Defender SmartScreen](/windows/security/threat-protection/microsoft-defender-smartscreen/microsoft-defender-smartscreen-overview)

## SmartScreen for Microsoft Edge URL scenario demonstrations

### Is This Phishing?

Alerts the user to a suspicious page and ask for feedback:

- [Is this Phishing?](https://demo.smartscreen.msft.net/other/areyousure.html)

  Launching this link should render a message similar to the following screenshot:

  :::image type="content" source="media/smartscreen-url-reputation-is-this-phishing.png" alt-text="SmartScreen alerts the user the site is potentially a phishing site and possibly unsafe":::

### Phishing Page

A page known for phishing that should be blocked:

- [A known Phishing page](https://demo.smartscreen.msft.net/phishingdemo.html)

  Launching this link should render a message similar to the following example:

  :::image type="content" source="media/smartscreen-url-reputation-this-is-phishing.png" alt-text="SmartScreen reports the site is known for containing phishing threats":::

### Malware page

A page that hosts malware and should be blocked:

- [A known malware page](https://demo.smartscreen.msft.net/other/malware.html)

  Launching this link should render a message similar to the following screenshot:

  :::image type="content" source="media/smartscreen-url-reputation-malware-page.png" alt-text="SmartScreen alerts the user that the site is know for containing harmful programs":::

### Blocked download

Blocked from downloading because of its URL reputation

- [Download blocked due to URL reputation](https://demo.smartscreen.msft.net/download/malwaredemo/freevideo.exe)

  Launching this link should render a message similar to the Malware page message.

### Exploit page

A page that attacks a browser vulnerability

- [Known browser exploit page](https://demo.smartscreen.msft.net/other/exploit.html)

  Launching this link should render a message similar to the Malware page message.

### Malvertising

A benign page hosting a malicious advertisement

- [A page known to contain malicious advertisements](https://demo.smartscreen.msft.net/other/exploit_frame.html)

  Launching this link should render a message similar to the following screenshot:

  :::image type="content" source="media/smartscreen-url-reputation-malvertising.png" alt-text="A demonstration of how SmartScreen responds to a frame on a page that is detected to be malicious. Only the malicious frame is blocked":::

## See also

[Microsoft Defender SmartScreen Documentation](/windows/security/threat-protection/microsoft-defender-smartscreen/microsoft-defender-smartscreen-overview)

[Microsoft Defender for Endpoint - demonstration scenarios](defender-endpoint-demonstrations.md)
[!INCLUDE [Microsoft Defender for Endpoint Tech Community](../../includes/defender-mde-techcommunity.md)]
