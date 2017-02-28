# Can I Subsystem It?

Compiling a list of web development dependencies and their support on the Windows Subsystem for Linux (aka Bash on Ubuntu on Windows). 

| App | Stable | Insider (Fast) | Notes |
|-----|--------|----------------|-------|
| [Gulp](http://gulpjs.com/)            |❌|✅||
| [Jekyll](http://jekyllrb.com/)        |❌|✅||
| [Karma](https://karma-runner.github.io/1.0/index.html) |❌|❌||
| [Libsass](http://sass-lang.com/libsass)                |❌|❌||
| [n](https://github.com/tj/n)          ||✅||
| [ngrok](https://ngrok.com/)           |❌|❌||
| [Node.js](https://nodejs.org/en/)     |❌|✅||
| [node-sass](https://github.com/sass/node-sass) |❌|❌||
| [npm](https://www.npmjs.com/)            |✅|✅||
| [nvm](https://github.com/creationix/nvm) |✅|✅|Causes slow Bash start times|
| [rbenv](https://github.com/rbenv/rbenv)  |✅|✅||
| [Ruby](https://www.ruby-lang.org/)       |✅|✅||
| [Ruby on Rails](http://rubyonrails.org/) |✅|✅||

<small>"Stable" refers to the Windows 10 Anniversary Update.</small>

## Known issues

There are some known overarching issues that affect a broad range of programs:

- Editing Linux files in Windows apps results in data corruption. [See blog post](https://blogs.msdn.microsoft.com/commandline/2016/11/17/do-not-change-linux-files-using-windows-apps-and-tools/).
- Node.js Network Interface ([#468](https://github.com/Microsoft/BashOnWindows/issues/468) _FIXED IN INSIDER_)
- NETLINK and ICMP ([#69](https://github.com/Microsoft/BashOnWindows/issues/69) _FIXED IN INSIDER_)
- INOTIFY filewatching ([#216](https://github.com/Microsoft/BashOnWindows/issues/216) _FIXED IN INSIDER_)

## Contributing

Yes, please. Probably need screenshots or console output to verify that it's working as expected.
