---
UID: NF:certenroll.IX509Enrollment.Enroll
title: IX509Enrollment::Enroll (certenroll.h)
description: Encodes a request, submits it to an appropriate certification authority (CA), and installs the response.
old-location: security\ix509enrollment_enroll_method.htm
tech.root: seccertenroll
ms.assetid: 63abecac-39f4-497a-8851-7a2260abc3dd
ms.date: 12/05/2018
ms.keywords: Enroll, Enroll method [Security], Enroll method [Security],IX509Enrollment interface, IX509Enrollment interface [Security],Enroll method, IX509Enrollment.Enroll, IX509Enrollment::Enroll, certenroll/IX509Enrollment::Enroll, security.ix509enrollment_enroll_method
ms.topic: method
f1_keywords:
- certenroll/IX509Enrollment.Enroll
dev_langs:
- c++
req.header: certenroll.h
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
req.lib: 
req.dll: CertEnroll.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- CertEnroll.dll
api_name:
- IX509Enrollment.Enroll
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IX509Enrollment::Enroll


## -description


The <b>Enroll</b> method encodes a request, submits it to an appropriate certification authority (CA), and installs the response.


## -parameters






## -returns



If the function succeeds, the function returns <b>S_OK</b>.

If the function fails, it returns an <b>HRESULT</b> value that indicates the error. Possible values include, but are not limited to, those in the following table. For a list of common error codes, see <a href="https://docs.microsoft.com/windows/desktop/SecCrypto/common-hresult-values">Common HRESULT Values</a>.

<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>OLE_E_BLANK</b></b></dt>
<dt></dt>
</dl>
</td>
<td width="60%">
The enrollment object has not been initialized.

</td>
</tr>
</table>
 




## -remarks



The method may create a key pair if necessary. Depending on how you initialize the enrollment object and on what properties you set, there may be no need to create a key pair. For example, if you are renewing a certificate by using an existing key, or if the <a href="https://docs.microsoft.com/windows/desktop/api/certenroll/nn-certenroll-ix509privatekey">IX509PrivateKey</a> object associated with the certificate request represents an existing key, this method does not create a new key pair.

Before enrolling, you must initialize the <a href="https://docs.microsoft.com/windows/desktop/api/certenroll/nn-certenroll-ix509enrollment">IX509Enrollment</a> object by calling one of the following methods.<ul>
<li>
<a href="https://docs.microsoft.com/windows/desktop/api/certenroll/nf-certenroll-ix509enrollment-initialize">Initialize</a>
</li>
<li>
<a href="https://docs.microsoft.com/windows/desktop/api/certenroll/nf-certenroll-ix509enrollment-initializefromrequest">InitializeFromRequest</a>
</li>
<li>
<a href="https://docs.microsoft.com/windows/desktop/api/certenroll/nf-certenroll-ix509enrollment-initializefromtemplatename">InitializeFromTemplateName</a>
</li>
</ul>


If the enrollment operation succeeds, the function  returns <b>S_OK</b>. However, this does not necessarily mean that the response from the CA was installed. Call  the <a href="https://docs.microsoft.com/windows/desktop/api/certenroll/nf-certenroll-ix509enrollment-get_status">Status</a> property to determine the enrollment status.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/certenroll/nn-certenroll-ix509enrollment">IX509Enrollment</a>
 

 

