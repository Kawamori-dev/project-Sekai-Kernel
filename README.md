# project: Sekai Kernel <br>

#### Description:
When I was younger I tried x86 architecture assembly and wrote boot loader to run code in real mode. <br>
And one megabyte felt like a whole universe for a lonely one, universe where I could create everything. <br>

Not far ago I started working on MMO RPG video game called "Dark Swordland Online". It's giant project and it can be downloaded in it's branch if already released as demo. <br>

The **"Project: Sekai Kernel"** is an engine of "Dark Swordland Online". At some point I noticed that game engine became somehow looks like it's an Operating system inside another Operating System. <br>

#### Some interesting solutions:
- Every piece of world can be changed without game server process restart. <br>
I called it HRT aka "Hot Reloadable Threads". The "Kernel" component reacts on changing (by checking timestamp of last change) in source files and re-compiles them automatically.
- Minimal dependents, cross-platform client.<br>
I used minimal amount of dependents. Main dependency is SDL2 - I use it to avoid suspicion of keylogging and window creating. I just get Framebuffer of the window and do render on my own.
I also made client work on Windows as well as on any POSIX Operating System. <br>
- Fast, Reliable Custom Networking Protocol.
Hah. I did my engine send HTTP 1.1/ 503th code "Forbidden" to everyone who tries to send packages without required signature and drop connection. It helps avoid to lost time on parsing garbage like scanner, spam bots and etc. <br>

#### I am careful about some details:
I dunno will I share my Game Engine with humans or not, but if so I did good logging: <br>

<img src="https://i.ibb.co/gMJyMdvB/picture-0.png" alt="drawing" width="80%" height="auto"/>

#### Roadmap:
- [x] Boot Sekai kernel for first time
- [x] Make client code Posix Standard and Windows NT compatiable
- [x] Create Custom Networking protocol
- [ ] Create Sekai messanging system (ITCP Inter Thread Communication Protocol API)
- [ ] Create Hot Reloadable Threads API 
- [ ] Create Render  

#### Release (approx) in: 28 days
