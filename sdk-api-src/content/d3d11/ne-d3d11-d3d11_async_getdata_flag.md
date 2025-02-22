---
UID: NE:d3d11.D3D11_ASYNC_GETDATA_FLAG
title: D3D11_ASYNC_GETDATA_FLAG (d3d11.h)
description: Optional flags that control the behavior of ID3D11DeviceContext::GetData.
old-location: direct3d11\d3d11_async_getdata_flag.htm
tech.root: direct3d11
ms.assetid: e2e40719-58ff-4440-b162-34f5edee021d
ms.date: 12/05/2018
ms.keywords: D3D11_ASYNC_GETDATA_DONOTFLUSH, D3D11_ASYNC_GETDATA_FLAG, D3D11_ASYNC_GETDATA_FLAG enumeration [Direct3D 11], cdcec50d-b059-b1bc-451c-42024bc0ed26, d3d11/D3D11_ASYNC_GETDATA_DONOTFLUSH, d3d11/D3D11_ASYNC_GETDATA_FLAG, direct3d11.d3d11_async_getdata_flag
ms.topic: enum
f1_keywords:
- d3d11/D3D11_ASYNC_GETDATA_FLAG
dev_langs:
- c++
req.header: d3d11.h
req.include-header: 
req.target-type: Windows
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
- APIRef
- kbSyntax
api_type:
- HeaderDef
api_location:
- D3D11.h
api_name:
- D3D11_ASYNC_GETDATA_FLAG
targetos: Windows
req.typenames: D3D11_ASYNC_GETDATA_FLAG
req.redist: 
ms.custom: 19H1
---

# D3D11_ASYNC_GETDATA_FLAG enumeration


## -description


Optional flags that control the behavior of <a href="https://docs.microsoft.com/windows/desktop/api/d3d11/nf-d3d11-id3d11devicecontext-getdata">ID3D11DeviceContext::GetData</a>.


## -enum-fields




### -field D3D11_ASYNC_GETDATA_DONOTFLUSH

Do not flush the command buffer. This can potentially cause an infinite loop if GetData is continually called until it returns S_OK as there may still be commands in the command buffer that need to be processed in order for GetData to return S_OK. Since the commands in the command buffer are not flushed they will not be processed and therefore GetData will never return S_OK.


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/direct3d11/d3d11-graphics-reference-d3d11-core-enums">Core Enumerations</a>
 

 

