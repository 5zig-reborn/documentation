# Chat Filter Placeholders
Chat Filter, Auto Text, and Join Auto Text support many different placeholders that are automatically evaluated by the mod.  
All placeholders have the `${placeholder}` syntax. For example, the `username` placeholder would be `${username}`.  
Here's a list:

## Player Coordinates
**Syntax**: `${coords}`  
User's coordinates, in the form of `X, Y, Z`.

## Player X Coordinate
**Syntax**: `${coordX}`

## Player Y Coordinate
**Syntax**: `${coordY}`

## Player Z Coordinate
**Syntax**: `${coordZ}`

## System Clipboard
**Syntax**: `${clipboard}`  
Acts as a normal paste action (Ctrl+V)

## Random entry in list
**Syntax**: `${random[entries]}`, example: `${random["Entry 1", "Entry 2", "Entry 3"]}`  
Selects a random entry from `entries`

## Current Server IP
**Syntax**: `${server-ip}`

## Current Server Lobby

!!! note
    Only available if the mod supports the server, either natively or via a plugin.
**Syntax**: `${server-lobby}`

## Current Server Port
**Syntax**: `${server-port}`

## Current Server Gamemode

!!! note
    Only available if the mod supports the server, either natively or via a plugin.
**Syntax**: `${server-gamemode}`

## Time (HH:mm)
**Syntax**: `${time-min}`

## Time (HH\:mm\:ss)
**Syntax**: `${time-sec}`

## Player Username
**Since**: 3.13.1  
**Syntax**: `${username}`

## Player UUID
**Since**: 3.13.1  
**Syntax**: `${uuid}`  
User's UUID *with* dashes. Example: `bba224a2-0bff-4913-b042-27ca3b60973f`

## Player UUID, stripped
**Since**: 3.13.1  
**Syntax**: `${uuid-stripped}`  
User's UUID *without* dashes. Example: `bba224a20bff4913b04227ca3b60973f`