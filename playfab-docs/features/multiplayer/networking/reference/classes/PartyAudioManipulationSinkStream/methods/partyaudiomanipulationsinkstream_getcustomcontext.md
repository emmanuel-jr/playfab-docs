---
author: jdeweyMSFT
title: "PartyAudioManipulationSinkStream::GetCustomContext"
description: The PartyAudioManipulationSinkStream::GetCustomContext method retrieves the app's private context value previously associated with this stream object.
ms.author: jdewey
ms.topic: reference
ms.prod: playfab
ms.date: 02/10/2020
---

# PartyAudioManipulationSinkStream::GetCustomContext  

Retrieves the app's private, custom pointer-sized context value previously associated with this stream object.  

## Syntax  
  
```cpp
PartyError GetCustomContext(  
    void** customContext  
)  
```  
  
### Parameters  
  
**`customContext`** &nbsp; void**  
*output, may return nullptr*  
  
The output custom context.  
  
  
### Return value  
PartyError
  
```c_partyErrorSuccess``` if the call succeeded or an error code otherwise. The human-readable form of the error code can be retrieved via [PartyManager::GetErrorMessage()](../../PartyManager/methods/partymanager_geterrormessage.md).
  
## Remarks  
  
If no custom context has been set yet, the value pointed to by `customContext` is set to nullptr.
  
## Requirements  
  
**Header:** Party.h
  
## See also  
[PartyAudioManipulationSinkStream](../partyaudiomanipulationsinkstream.md)  
[PartyAudioManipulationSinkStream::SetCustomContext](partyaudiomanipulationsinkstream_setcustomcontext.md)
  
  
