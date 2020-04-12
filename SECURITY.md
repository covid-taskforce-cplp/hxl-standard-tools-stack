# Security Policy

<!-- TOC -->

- [Security Policy](#security-policy)
    - [The test server](#the-test-server)
        - [Can I log in with the administrative panels docummented on the README.md?](#can-i-log-in-with-the-administrative-panels-docummented-on-the-readmemd)
    - [Supported Versions](#supported-versions)
    - [Reporting a Vulnerability](#reporting-a-vulnerability)
        - [About the test server or the stack](#about-the-test-server-or-the-stack)
        - [Via e-mail](#via-e-mail)

<!-- /TOC -->

## The test server

For some period of time, this project may have a public test server at
`hxl.etica.dev`. **You are free to make security testing on this test server**
and then use the [Reporting a Vulnerability](#reporting-a-vulnerability).

### Can I log in with the administrative panels docummented on the README.md?

Yes! At least for some active period, we may even release the Portainer admin
password on the [README.md file](README.md). **Just don't troll intentionally**
but it's ok if you break something, since the server can be recreated from
scratch with the Ansible.

## Supported Versions

The `covid-taskforce-cplp/hxl-standard-tools-stack` is unlikely to have stable
releases considering that the user base may be low.

But you are still encoraged to report or make suggestions if you may consider
use this as part of other projects

## Reporting a Vulnerability

### About the test server or the stack

If what you are reporting is the stack itself (and is not about we intentionally
relase some admin access on the readme file **if** this does not allow automated
exploits) you can make public comments on the issues page
[covid-taskforce-cplp/hxl-standard-tools-stack/issues](https://github.com/covid-taskforce-cplp/hxl-standard-tools-stack/issues).

If the issue may affect some of the software on this stack and potentially
productions servers that are hosted by humanitarian organizations, if you want
to be explicity, consider do it via e-mail.

### Via e-mail

In special if a vunerability may affect a production server, even if was
discovered on our test servers, please contact some of the authors directly. One
possible contact is: _Emerson Rocha <rocha@ieee.org>_ via e-mail.
