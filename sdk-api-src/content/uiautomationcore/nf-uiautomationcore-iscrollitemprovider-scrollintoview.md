---
UID: NF:uiautomationcore.IScrollItemProvider.ScrollIntoView
title: IScrollItemProvider::ScrollIntoView (uiautomationcore.h)
description: Scrolls the content area of a container object in order to display the control within the visible region (viewport) of the container.
old-location: winauto\uiauto_IScrollItemProvider_ScrollIntoView.htm
tech.root: WinAuto
ms.assetid: 2d1ce9f2-b3ba-40c5-a750-bd739b1abc07
ms.date: 12/05/2018
ms.keywords: IScrollItemProvider interface [Windows Accessibility],ScrollIntoView method, IScrollItemProvider.ScrollIntoView, IScrollItemProvider::ScrollIntoView, ScrollIntoView, ScrollIntoView method [Windows Accessibility], ScrollIntoView method [Windows Accessibility],IScrollItemProvider interface, uiauto.uiauto_IScrollItemProvider_ScrollIntoView, uiauto_IScrollItemProvider_ScrollIntoView, uiautomationcore/IScrollItemProvider::ScrollIntoView, winauto.uiauto_IScrollItemProvider_ScrollIntoView
ms.topic: method
f1_keywords:
- uiautomationcore/IScrollItemProvider.ScrollIntoView
dev_langs:
- c++
req.header: uiautomationcore.h
req.include-header: UIAutomation.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: UIAutomationCore.idl
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
- COM
api_location:
- UIAutomationCore.h
api_name:
- IScrollItemProvider.ScrollIntoView
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IScrollItemProvider::ScrollIntoView


## -description


Scrolls the content area of a container object in order to display the control within the visible region (viewport) of the container.
        


## -parameters






## -returns



Type: <b><a href="https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



This method will not guarantee the position of the control 
            within the visible region (viewport) of the container.
            




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/uiautomationcore/nn-uiautomationcore-iscrollitemprovider">IScrollItemProvider</a>



<a href="https://docs.microsoft.com/windows/desktop/WinAuto/uiauto-providersoverview">UI Automation Providers Overview</a>
 

 

