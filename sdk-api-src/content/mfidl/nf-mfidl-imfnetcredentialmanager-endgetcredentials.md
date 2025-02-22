---
UID: NF:mfidl.IMFNetCredentialManager.EndGetCredentials
title: IMFNetCredentialManager::EndGetCredentials (mfidl.h)
description: Completes an asynchronous request to retrieve the user's credentials.
old-location: mf\imfnetcredentialmanager_endgetcredentials.htm
tech.root: medfound
ms.assetid: 99914ded-1b9a-4373-9974-e1d1b1abd4e2
ms.date: 12/05/2018
ms.keywords: 99914ded-1b9a-4373-9974-e1d1b1abd4e2, EndGetCredentials, EndGetCredentials method [Media Foundation], EndGetCredentials method [Media Foundation],IMFNetCredentialManager interface, IMFNetCredentialManager interface [Media Foundation],EndGetCredentials method, IMFNetCredentialManager.EndGetCredentials, IMFNetCredentialManager::EndGetCredentials, mf.imfnetcredentialmanager_endgetcredentials, mfidl/IMFNetCredentialManager::EndGetCredentials
ms.topic: method
f1_keywords:
- mfidl/IMFNetCredentialManager.EndGetCredentials
dev_langs:
- c++
req.header: mfidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mfuuid.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- mfuuid.lib
- mfuuid.dll
api_name:
- IMFNetCredentialManager.EndGetCredentials
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IMFNetCredentialManager::EndGetCredentials


## -description



Completes an asynchronous request to retrieve the user's credentials.




## -parameters




### -param pResult [in]

Pointer to an <a href="https://docs.microsoft.com/windows/desktop/api/mfobjects/nn-mfobjects-imfasyncresult">IMFAsyncResult</a> interface that contains the asynchronous result.


### -param ppCred [out]

Receives a pointer to the <a href="https://docs.microsoft.com/windows/desktop/api/mfidl/nn-mfidl-imfnetcredential">IMFNetCredential</a> interface, which is used to retrieve the credentials. The caller must release the interface.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>
 




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/mfidl/nn-mfidl-imfnetcredentialmanager">IMFNetCredentialManager</a>
 

 

