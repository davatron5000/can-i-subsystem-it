# Can I Subsystem It?

Compiling a list of web development dependencies and their support on the Windows Subsystem for Linux (aka Bash on Ubuntu on Windows). 

| App | Anniversary Update | Insider (Fast) | Notes |
|-----|--------|----------------|-------|
| [Gulp](http://gulpjs.com/)                  |❌|✅||
| [Haskell](https://blogs.msdn.microsoft.com/commandline/2017/02/09/haskell-on-bashwsl/) |❌|✅||
| [hub](https://github.com/github/hub)        |❌|❌|[hostname bug](https://github.com/Microsoft/BashOnWindows/issues/562) fixed in Insider, still fails silently|
| [Hyper](http://hyper.is/)                   |❌|❌|[Up arrow doesn't work](https://github.com/zeit/hyper/issues/1127)|
| [Java](https://www.java.com/)               |❌|✅||
| [JDK7](http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html)     |✅|✅||
| [JDK8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)     |❌|✅||
| [Jekyll](http://jekyllrb.com/)              |❌|✅||
| [Karma](https://karma-runner.github.io/1.0/index.html) |❌|❌||
| [LevelDB](https://github.com/level/level)   ||✅||
| [Libsass](http://sass-lang.com/libsass)     ||✅||
| [MySQL](https://mysql.com/)                 |❌|✅||
| [n](https://github.com/tj/n)                ||✅||
| [ngrok](https://ngrok.com/)                 |❌|❌||
| [Node.js](https://nodejs.org/en/)           |❌|✅||
| [node-sass](https://github.com/sass/node-sass) ||✅||
| [node-sqlite3](https://github.com/mapbox/node-sqlite3) |❌|❌||
| [npm](https://www.npmjs.com/)               |✅|✅||
| [nvm](https://github.com/creationix/nvm)    |✅|✅|Causes slow Bash start times|
| [Oh My Zsh](http://ohmyz.sh/)               |✅|✅|Some themes don't render well|
| [PostgreSQL](https://www.postgresql.org//)  |❌|✅||
| [rbenv](https://github.com/rbenv/rbenv)     |✅|✅||
| [Ruby](https://www.ruby-lang.org/)          |✅|✅||
| [Ruby on Rails](http://rubyonrails.org/)    |✅|✅||
| [SAMBA](https://www.samba.org/~garming/)    |❌|✅||
| [sshd](https://en.wikipedia.org/wiki/Secure_Shell) |❌|✅||
| [zsh](http://www.zsh.org/)                  |✅|✅||

## Known issues
There are some known overarching issues that affect a broad range of programs:

- Disk IO perf is relatively slow. If you run disk-intensive operations (e.g. restoring a large Git repo and/or projects with lots of node modules / Ruby Gems), you'll likely see slower performance than on native Ubuntu. The team are aware of this issue and are working to remedy in future OS releases.
- Editing Linux files in Windows apps results in data corruption. [See blog post](https://blogs.msdn.microsoft.com/commandline/2016/11/17/do-not-change-linux-files-using-windows-apps-and-tools/).
- Node.js Network Interface ([#468](https://github.com/Microsoft/BashOnWindows/issues/468) _FIXED IN INSIDER_)
- NETLINK and ICMP ([#69](https://github.com/Microsoft/BashOnWindows/issues/69) _FIXED IN INSIDER_)
- INOTIFY filewatching ([#216](https://github.com/Microsoft/BashOnWindows/issues/216) _FIXED IN INSIDER_)
- Shared Memory support (required by Postgres, etc.) ([#61](https://github.com/Microsoft/BashOnWindows/issues/61) _FIXED IN INSIDER_)

> See [WSL Release Notes](https://msdn.microsoft.com/commandline/wsl/release_notes) for more details of specific issued fixed, and syscalls added

## Contributing
Yes, please. Probably need screenshots or console output to verify that it's working as expected.
