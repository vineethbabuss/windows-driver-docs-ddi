---
UID: NC:d3dumddi.PFND3DDDI_CREATEEXTENSIONDEVICE
title: PFND3DDDI_CREATEEXTENSIONDEVICE
author: windows-driver-content
description: The CreateExtensionDevice function creates a Microsoft DirectX Video Acceleration (DirectX VA) extension device.
old-location: display\createextensiondevice.htm
tech.root: display
ms.assetid: 7e6dbb70-2e74-4ddb-a504-2c8145af99d9
ms.date: 05/10/2018
ms.keywords: CreateExtensionDevice, CreateExtensionDevice callback function [Display Devices], PFND3DDDI_CREATEEXTENSIONDEVICE, PFND3DDDI_CREATEEXTENSIONDEVICE callback, UserModeDisplayDriver_Functions_342ee084-e24a-43a8-99a9-c83c2670e2e4.xml, d3dumddi/CreateExtensionDevice, display.createextensiondevice
ms.topic: callback
req.header: d3dumddi.h
req.include-header: D3dumddi.h
req.target-type: Desktop
req.target-min-winverclnt: Available in Windows Vista and later versions of the Windows operating systems.
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	UserDefined
api_location:
-	d3dumddi.h
api_name:
-	CreateExtensionDevice
product:
- Windows
targetos: Windows
req.typenames: 
---

# PFND3DDDI_CREATEEXTENSIONDEVICE callback function


## -description


The <b>CreateExtensionDevice</b> function creates a Microsoft DirectX Video Acceleration (DirectX VA) extension device. 


## -parameters




### -param hDevice [in]

A handle to the display device (graphics context).


### -param *








*pData* [in, out]

A pointer to a <a href="https://msdn.microsoft.com/library/windows/hardware/ff542938">D3DDDIARG_CREATEEXTENSIONDEVICE</a> structure. On input, this structure contains information that the driver can use. On output, the driver specifies information in the structure that the Microsoft Direct3D runtime can use.


## -returns



<b>CreateExtensionDevice</b> returns one of the following values:

| **Return code** | **Description** | 
|:--|:--|
| **S_OK** | The extension device is successfully created. | 
| **E_OUTOFMEMORY** | [CreateExtensionDevice](https://msdn.microsoft.com/7e6dbb70-2e74-4ddb-a504-2c8145af99d9)  could not allocate the required memory for it to complete. | 





## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff542938">D3DDDIARG_CREATEEXTENSIONDEVICE</a>



<a href="https://msdn.microsoft.com/8c4bcab3-b903-4f39-aab0-7efb3b18d068">DestroyExtensionDevice</a>
 

 

