---
UID: NF:ntintsafe.RtlPtrdiffTAdd
title: RtlPtrdiffTAdd function
author: windows-driver-content
description: Adds two values of type PTRDIFF_T.
old-location: kernel\rtlptrdifftadd.htm
tech.root: kernel
ms.assetid: 3B4C0CF0-8153-446E-A834-C1FE28651718
ms.date: 04/30/2018
ms.keywords: RtlPtrdiffTAdd, RtlPtrdiffTAdd function [Kernel-Mode Driver Architecture], kernel.rtlptrdifftadd, ntintsafe/RtlPtrdiffTAdd
ms.topic: function
req.header: ntintsafe.h
req.include-header: 
req.target-type: Desktop
req.target-min-winverclnt: 
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
-	HeaderDef
api_location:
-	Ntintsafe.h
api_name:
-	RtlPtrdiffTAdd
product:
- Windows
targetos: Windows
req.typenames: 
---

# RtlPtrdiffTAdd function


## -description


Adds two values of type <b>PTRDIFF_T</b>.


## -parameters




### -param Augend [in]

The first value in the equation.


### -param Addend [in]

The value to add to <i>Augend</i>.


### -param pResult [out]

A pointer to the sum. If the operation results in a value that overflows or underflows the capacity of the type, the function returns STATUS_INTEGER_OVERFLOW and this parameter is not valid.


## -remarks



This is one of a set of inline functions designed to provide arithmetic operations and perform validity checks with minimal impact on performance.



