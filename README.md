**:point_right: No Longer Maintained :point_left:**

*The Eclipse Git integration is considering moving away from JSch. This project is therefore no longer maintained.*

Please help building an ssh-agent integration for the Eclipse Git. [Details at bug 541274](https://bugs.eclipse.org/bugs/show_bug.cgi?id=541274)

---

# Eclipse ssh-agent and Pageant support

This project provides Eclipse Plug-ins to use [OpenSSH](http://www.openssh.com/)'s [ssh-agent](http://en.wikipedia.org/wiki/Ssh-agent)
and [Pageant](http://en.wikipedia.org/wiki/PuTTY#Applications) in Eclipse.

Provided plug-ins depend on [jsch-agent-proxy](http://www.jcraft.com/jsch-agent-proxy/). This is an effort for [Bug179924](https://bugs.eclipse.org/bugs/show_bug.cgi?id=179924).


## Install
1.   Help > Install New Software...

     Work with: https://eclipseguru.github.io/eclipse-jsch-agent-proxy/
     ![install software screenshot](https://raw.githubusercontent.com/eclipseguru/eclipse-jsch-agent-proxy/gh-pages/images/install-software.png "Install New Software Dialog")

2.   Restart Eclipse

3.   Choose the ssh agent you want to use

     Window > Preferences > General > Network Connections > SSH2 > SSH Agent
     ![ssh agent preferences screenshot](https://raw.githubusercontent.com/eclipseguru/eclipse-jsch-agent-proxy/gh-pages/images/ssh-agent-preferences.png "SSH Agent Preferences")

4.   Remove all configured private keys (otherwise Eclipse keeps asking for passphrases)

     Window > Preferences > General > Network Connections > SSH2 > SSH Agent
     ![ssh no private keys preferences screenshot](https://raw.githubusercontent.com/eclipseguru/eclipse-jsch-agent-proxy/gh-pages/images/no-private-keys.png "No Private Keys Preferences")

## License
This software is licensed under revised BSD license, and depends on other software.

* com.jcraft.jsch.agentproxy.eclipse.pageant is using [JNA](https://github.com/twall/jna), which is licensed under [Apache License, Version 2.0](https://github.com/twall/jna/blob/master/LICENSE).
* com.jcraft.jsch.agentproxy.eclipse.sshagent is using [JNA](https://github.com/twall/jna), which is licensed under [Apache License, Version 2.0](https://github.com/twall/jna/blob/master/LICENSE).

