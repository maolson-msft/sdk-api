---
UID: NE:virtdisk._DELETE_SNAPSHOT_VHDSET_FLAG
title: DELETE_SNAPSHOT_VHDSET_FLAG (virtdisk.h)
description: Contains flags affecting the behavior of the DeleteSnapshotVhdSet function.
old-location: vhd\delete_snapshot_vhdset_flag.htm
tech.root: VStor
ms.assetid: 42B56389-8ECE-4127-A641-7F0A0A1E7D2D
ms.date: 12/05/2018
ms.keywords: '*PDELETE_SNAPSHOT_VHDSET_FLAG, DELETE_SNAPSHOT_VHDSET_FLAG, DELETE_SNAPSHOT_VHDSET_FLAG enumeration [VHD], DELETE_SNAPSHOT_VHDSET_FLAG_NONE, DELETE_SNAPSHOT_VHDSET_FLAG_PERSIST_RCT, PDELETE_SNAPSHOT_VHDSET_FLAG, PDELETE_SNAPSHOT_VHDSET_FLAG enumeration pointer [VHD], vdssys/DELETE_SNAPSHOT_VHDSET_FLAG, vdssys/DELETE_SNAPSHOT_VHDSET_FLAG_NONE, vdssys/DELETE_SNAPSHOT_VHDSET_FLAG_PERSIST_RCT, vdssys/PDELETE_SNAPSHOT_VHDSET_FLAG, vhd.delete_snapshot_vhdset_flag, virtdisk/DELETE_SNAPSHOT_VHDSET_FLAG, virtdisk/DELETE_SNAPSHOT_VHDSET_FLAG_NONE, virtdisk/DELETE_SNAPSHOT_VHDSET_FLAG_PERSIST_RCT, virtdisk/PDELETE_SNAPSHOT_VHDSET_FLAG'
ms.topic: enum
f1_keywords:
- virtdisk/DELETE_SNAPSHOT_VHDSET_FLAG
dev_langs:
- c++
req.header: virtdisk.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
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
- VirtDisk.h
- vdssys.h
api_name:
- DELETE_SNAPSHOT_VHDSET_FLAG
targetos: Windows
req.typenames: DELETE_SNAPSHOT_VHDSET_FLAG, *PDELETE_SNAPSHOT_VHDSET_FLAG
req.redist: 
ms.custom: 19H1
---

# DELETE_SNAPSHOT_VHDSET_FLAG enumeration


## -description


<p class="CCE_Message">[Some information relates to pre-released product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.]

Contains flags affecting the behavior of the <a href="https://docs.microsoft.com/windows/win32/api/virtdisk/nf-virtdisk-deletesnapshotvhdset">DeleteSnapshotVhdSet</a> function.


## -enum-fields




### -field DELETE_SNAPSHOT_VHDSET_FLAG_NONE

No flag specified.


### -field DELETE_SNAPSHOT_VHDSET_FLAG_PERSIST_RCT

A reference point should be persisted in the VHD Set after the snapshot is deleted.

