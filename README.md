# saltychat-altV
alt:V Version of Saltychat Plugin using C# Serverside

Fill in Serverside required Settings, compile the Serverside and add it to your server

For alt:V Specific Questions consider asking in [alt:V Discord](https://dscrd.in/altVMP)

How To Enable the Plugin on Connect:

This implementation needs an emit from Server and from saltychat.dll

If you use Javascript Serverside you need to emit 2 things:

```javascript
// Only after both Functions are emitted the Player will be moved

// This ones for SaltyChat.dll to apply player
// This has to be sent from Serverside anywhere in your Script
alt.emit("PlayerLoggedIn", player, playerName)

// This ones for the Client to confirm WebSocket has Connected
// Its already included in the SaltyWebSocket.html
alt.emit(player, "SaltyChat_OnConnected")
```
