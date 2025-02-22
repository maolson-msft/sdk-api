---
UID: NS:sspi._SecPkgCredentials_Cert
title: SecPkgCredentials_Cert (sspi.h)
description: Specifies the certificate credentials. The QueryCredentialsAttributes function uses this structure.
old-location: security\secpkgcredentials_cert.htm
tech.root: SecAuthN
ms.assetid: 9EEE6E98-D45C-4929-9C9C-F344972D186F
ms.date: 12/05/2018
ms.keywords: '*PSecPkgCredentials_Cert, PSecPkgCredentials_Cert, PSecPkgCredentials_Cert structure pointer [Security], SecPkgCredentials_Cert, SecPkgCredentials_Cert structure [Security], security.secpkgcredentials_cert, sspi/PSecPkgCredentials_Cert, sspi/SecPkgCredentials_Cert'
ms.topic: struct
f1_keywords:
- sspi/SecPkgCredentials_Cert
dev_langs:
- c++
req.header: sspi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2003 R2 [desktop apps only]
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
- Sspi.h
api_name:
- SecPkgCredentials_Cert
targetos: Windows
req.typenames: SecPkgCredentials_Cert, *PSecPkgCredentials_Cert
req.redist: 
ms.custom: 19H1
---

# SecPkgCredentials_Cert structure


## -description


Specifies the certificate credentials. The <a href="https://docs.microsoft.com/windows/desktop/api/sspi/nf-sspi-querycredentialsattributesa">QueryCredentialsAttributes</a> function uses this structure.


## -struct-fields




### -field EncodedCertSize

Size of the encoded certificate.


### -field EncodedCert

The encoded certificate.

