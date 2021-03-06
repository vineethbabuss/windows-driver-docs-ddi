---
UID: NS:netpacket._NET_PACKET_LARGE_SEND_SEGMENTATION
title: _NET_PACKET_LARGE_SEND_SEGMENTATION
author: windows-driver-content
description: The NET_PACKET_LARGE_SEND_SEGMENTATION structure contains large send offload (LSO) information for a packet.
tech.root: netvista
ms.assetid: a6483202-e3e4-48d9-86fa-42f21d57206f
ms.date: 03/02/2018
ms.topic: struct
ms.keywords: _NET_PACKET_LARGE_SEND_SEGMENTATION, NET_PACKET_LARGE_SEND_SEGMENTATION, 
req.header: netpacket.h
req.include-header: netadaptercx.h
req.target-type:
req.target-min-winverclnt:
req.target-min-winversvr:
req.kmdf-ver: 1.25
req.umdf-ver:
req.lib:
req.dll:
req.ddi-compliance:
req.unicode-ansi:
req.max-support:
req.typenames: NET_PACKET_LARGE_SEND_SEGMENTATION
topictype: 
-	apiref
apitype: 
-	HeaderDef
apilocation: 
-	netpacket.h
apiname: 
-	_NET_PACKET_LARGE_SEND_SEGMENTATION
product:
-	Windows
targetos: Windows
---

# _NET_PACKET_LARGE_SEND_SEGMENTATION structure

## -description
> [!WARNING]
> Some information in this topic relates to prereleased product, which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.
>
> NetAdapterCx is preview only in Windows 10, version 1809.

The **NET_PACKET_LARGE_SEND_SEGMENTATION** structure contains large send offload (LSO) information for a packet.

## -struct-fields

### -field DUMMYUNIONNAME
A union that contains the **TCP** member.

### -field DUMMYUNIONNAME.TCP
A structure that holds the TCP LSO information.

### -field DUMMYUNIONNAME.TCP.Mss
The maximum segment size (MSS) for TCP segments.
 
### -field DUMMYUNIONNAME.TCP.Reserved0
Reserved for system use. Clients must not read or write this member.

## -remarks
Client drivers can obtain this structure for a packet by calling [NetPacketGetPacketLargeSendSegmentation](nf-netpacket-netpacketgetpacketlargesendsegmentation.md).



## -see-also

[Packet descriptors and extensions](https://docs.microsoft.com/windows-hardware/drivers/netcx/packet-descriptors-and-extensions)
