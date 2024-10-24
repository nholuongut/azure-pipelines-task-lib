
# Azure Pipelines Task SDK

![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

Libraries for writing [Azure Pipelines](https://azure.microsoft.com/en-us/services/devops/pipelines) tasks

Reference examples of our in the box tasks [are here](https://github.com/Microsoft/azure-pipelines-tasks)

## TypeScript Tasks

Cross platform tasks are written in TypeScript.  It is the preferred way to write tasks once.

[![NPM version][npm-lib-image]][npm-lib-url]

Step by Step: [Create Task](https://docs.microsoft.com/en-us/azure/devops/extend/develop/add-build-task?view=vsts)

Documentation: [TypeScript API](https://github.com/nholuongut/azure-pipelines-task-lib/blob/master/node/docs/azure-pipelines-task-lib.md), [task JSON schema](https://aka.ms/vsts-tasks.schema.json)

Guidance: [Finding Files](https://github.com/nholuongut/azure-pipelines-task-lib/blob/master/node/docs/findingfiles.md), [Minimum agent version](https://github.com/nholuongut/azure-pipelines-task-lib/blob/master/node/docs/minagent.md), [Proxy](https://github.com/nholuongut/azure-pipelines-task-lib/blob/master/node/docs/proxy.md), [Certificate](https://github.com/nholuongut/azure-pipelines-task-lib/blob/master/node/docs/cert.md)

## Node 10 Upgrade Notice

Azure DevOps is currently working to establish Node 10 as the new preferred runtime for tasks, upgrading from Node 6.
Relevant work is happening in the `master` branch and the major version should be used with Node 10 is 3.
Previous major version is stored in the `releases/2.x`

### Upgrading to Node 10

Upgrading your tasks from Node 6 should be relatively painless, however there are some things to note:
* Typescript has been upgraded to TS 4. Older versions of TS may or may not work with Node 14 or the 3.x branch. We recommend upgrading to TS 4 when upgrading to task-lib 3.x.
* Node has made some changes to `fs` between Node 6 and Node 10. It is worth reviewing and testing your tasks thoroughly before publishing updates to Node 10.

## Reference Examples

The [ShellScript Task](https://github.com/Microsoft/azure-pipelines-tasks/tree/master/Tasks/ShellScriptV2) and the [XCode Task](https://github.com/Microsoft/azure-pipelines-tasks/tree/master/Tasks/XcodeV5) are good examples.

## Contributing

We are accepting contributions and we try to stay on top of issues.

[Contribution Guide](https://github.com/nholuongut/azure-pipelines-task-lib/blob/master/CONTRIBUTING.md).

[Logging Issues](https://github.com/nholuongut/azure-pipelines-task-lib/issues)

## Building the library

Once:
```bash
$ cd node
$ npm install
```

Build and Test:
```bash
$ npm test
```

Set environment variable TASK_TEST_TRACE=1 to display test output.

[npm-lib-image]: https://img.shields.io/npm/v/azure-pipelines-task-lib.svg?style=flat
[npm-lib-url]: https://www.npmjs.com/package/azure-pipelines-task-lib

## Powershell

We also maintain a PowerShell library for Windows task development.

Library: [Powershell Library](https://github.com/nholuongut/azure-pipelines-task-lib/tree/master/powershell)

Usage: [Consuming the SDK](https://github.com/nholuongut/azure-pipelines-task-lib/blob/master/powershell/Docs/Consuming.md)

## Third Party Notices
To generate/update third party notice file run:
```bash
$ node generate-third-party-notice.js
```

# 🚀 I'm are always open to your feedback.  Please contact as bellow information:
### [Contact ]
* [Name: nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License
* Nho Luong (c). All Rights Reserved.🌟