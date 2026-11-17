## 修复断开后断网 · Fixed losing internet after disconnecting

**中文**
- 修复：同时用过其他代理软件（如 Clash Verge、Clash for Young）时，断开后整台电脑可能连不上网
- 修复：断开时不再关掉其他正在使用的代理软件的系统代理
- 增强模式断开时等待内核清理完路由，避免残留路由导致断网

**English**
- Fixed: after using another proxy app (e.g. Clash Verge, Clash for Young), disconnecting could leave the whole computer offline
- Fixed: disconnecting no longer turns off the system proxy of another proxy app that's still in use
- Enhanced mode now waits for the core to clean up its routes when disconnecting, so leftover routes can't cut off the network
