---
UID: NF:shlwapi.SHRegSetUSValueW
title: SHRegSetUSValueW function (shlwapi.h)
description: Sets a registry subkey value in a user-specific subtree (HKEY_CURRENT_USER or HKEY_LOCAL_MACHINE).
old-location: shell\SHRegSetUSValue.htm
tech.root: shell
ms.assetid: 96559f8c-8527-4924-928e-f27049069407
ms.date: 12/05/2018
ms.keywords: SHREGSET_DEFAULT, SHREGSET_FORCE_HKCU, SHREGSET_FORCE_HKLM, SHREGSET_HKCU, SHREGSET_HKLM, SHRegSetUSValue, SHRegSetUSValue function [Windows Shell], SHRegSetUSValueA, SHRegSetUSValueW, _win32_SHRegSetUSValue, shell.SHRegSetUSValue, shlwapi/SHRegSetUSValue, shlwapi/SHRegSetUSValueA, shlwapi/SHRegSetUSValueW
ms.topic: function
f1_keywords:
- shlwapi/SHRegSetUSValue
dev_langs:
- c++
req.header: shlwapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional, Windows XP [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: SHRegSetUSValueW (Unicode) and SHRegSetUSValueA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Shlwapi.lib
req.dll: Shlwapi.dll (version 4.71 or later)
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Shlwapi.dll
- API-MS-Win-Core-Registryuserspecific-l1-1-0.dll
- KernelBase.dll
- API-MS-Win-DownLevel-shlwapi-l1-1-0.dll
- API-MS-Win-DownLevel-shlwapi-l1-1-1.dll
api_name:
- SHRegSetUSValue
- SHRegSetUSValueA
- SHRegSetUSValueW
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# SHRegSetUSValueW function


## -description


Sets a registry subkey value in a user-specific subtree (HKEY_CURRENT_USER or HKEY_LOCAL_MACHINE).


## -parameters




### -param pwzSubKey

TBD


### -param pwzValue

TBD


### -param dwType [in]

Type: <b>DWORD</b>

Type of data to be stored. This parameter must be the <b>REG_SZ</b> type. For more information, see <a href="https://docs.microsoft.com/windows/desktop/shell/schemas">Registry Data Types</a>.


### -param pvData [in, optional]

Type: <b>LPVOID*</b>

 Apointer to a null-terminated string that contains the value to be set for the specified key.


### -param cbData [in, optional]

Type: <b>DWORD</b>

Length, in bytes, of the string pointed to by the <i>pvData</i> parameter, not including the terminating null character.


### -param dwFlags [in, optional]

Type: <b>DWORD</b>

Flags indicating where the data should be written.



#### SHREGSET_HKCU

Write to <b>HKEY_CURRENT_USER</b> if empty.



#### SHREGSET_FORCE_HKCU

Write to <b>HKEY_CURRENT_USER</b>.



#### SHREGSET_HKLM

Write to <b>HKEY_LOCAL_MACHINE</b> if empty.



#### SHREGSET_FORCE_HKLM

Write to <b>HKEY_LOCAL_MACHINE</b>.



#### SHREGSET_DEFAULT

Equivalent to (<b>SHREGSET_FORCE_HKCU</b> | <b>SHREGSET_HKLM</b>).


##### - dwFlags.SHREGSET_DEFAULT

Equivalent to (<b>SHREGSET_FORCE_HKCU</b> | <b>SHREGSET_HKLM</b>).


##### - dwFlags.SHREGSET_FORCE_HKCU

Write to <b>HKEY_CURRENT_USER</b>.


##### - dwFlags.SHREGSET_FORCE_HKLM

Write to <b>HKEY_LOCAL_MACHINE</b>.


##### - dwFlags.SHREGSET_HKCU

Write to <b>HKEY_CURRENT_USER</b> if empty.


##### - dwFlags.SHREGSET_HKLM

Write to <b>HKEY_LOCAL_MACHINE</b> if empty.


#### - pszSubKey [in]

Type: <b>LPCTSTR</b>

A pointer to a null-terminated string with the name of the subkey.


#### - pszValue [in]

Type: <b>LPCTSTR</b>

A pointer to a null-terminated string that specifies the name of the value.


## -returns



Type: <b>LSTATUS</b>

Returns ERROR_SUCCESS if successful, or a nonzero error code defined in Winerror.h otherwise. You can use the <a href="https://docs.microsoft.com/windows/desktop/api/winbase/nf-winbase-formatmessage">FormatMessage</a> function with the FORMAT_MESSAGE_FROM_SYSTEM flag to retrieve a generic description of the error.




## -remarks



This function opens the key each time it is used. If your code involves setting a series of values in the same key, it is more efficient to open the key once with <a href="https://docs.microsoft.com/windows/desktop/api/shlwapi/nf-shlwapi-shregopenuskeya">SHRegOpenUSKey</a> and then use <a href="https://docs.microsoft.com/windows/desktop/api/shlwapi/nf-shlwapi-shregwriteusvaluea">SHRegWriteUSValue</a> to write the data.



