---
author: ScottMunroMS
title: "PFLobbyDisconnectedStateChange"
description: "Information specific to the *Disconnected* type of state change."
ms.author: scmunro
ms.topic: reference
ms.prod: playfab
ms.date: 01/03/2022
---

# PFLobbyDisconnectedStateChange  

Information specific to the *Disconnected* type of state change.  

## Syntax  
  
```cpp
typedef struct PFLobbyDisconnectedStateChange {  
    _Notnull_ lobby;  
} PFLobbyDisconnectedStateChange  
```
  
### Members  
  
**`lobby`** &nbsp; _Notnull_  
  
The lobby that has disconnected.
  
## Remarks  
  
This state change signals that the lobby has completed disconnecting. This is the last state change that will be provided for this lobby object. Once this state change is returned to [PFMultiplayerFinishProcessingLobbyStateChanges()](../functions/pfmultiplayerfinishprocessinglobbystatechanges.md), the Lobby object memory will become invalid.
  
## Requirements  
  
**Header:** PFLobby.h
  
## See also  
[PFLobby members](../pflobby_members.md)  

  
  
