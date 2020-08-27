Test Packages on Gitpod
=======================

To test packages for the **`latest ubuntu`** release, simple click on the badge below:

[![Gitpod](https://gitpod.io/button/open-in-gitpod.svg)][1]

Find out more on [YARP-enabled Gitpod workspaces][2].

Instead, if you aim to test against different **`distros/releases`**, do:
1. Edit the file [`.gitpod.Dockerfile`](/.gitpod.Dockerfile) and create a new branch. In detail, you have to fiddle with these [sections][3].
2. Launch the corresponding Gitpod workspace from within the new branch. Don't click on the main badge but rather customize the [URL context][4]. To ease this operation, you may install the [Gitpod browser extension][5].

⚠ As Docker relies on cached sections, you may still be using an old image when you've just updated a package to test. To invalidate the cache forcing Docker to build the relevant sections entirely again, apply this [workaround][6]. 


[1]: https://gitpod.io/#https://github.com/icub-tech-iit/test-packages-gitpod
[2]: https://spectrum.chat/icub/technicalities/yarp-enabled-gitpod-workspaces-available~73ab5ee9-830e-4b7f-9e99-195295bb5e34
[3]: https://github.com/icub-tech-iit/test-packages-gitpod/blob/master/.gitpod.Dockerfile#L1-L8
[4]: https://www.gitpod.io/docs/context-urls/#branch-context
[5]: https://www.gitpod.io/docs/browser-extension
[6]: https://github.com/icub-tech-iit/test-packages-gitpod/blob/master/.gitpod.Dockerfile#L94-L95
