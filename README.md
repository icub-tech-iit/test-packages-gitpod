Test Packages on Gitpod
=======================

To test packages for the **`latest ubuntu`** release simple click on the badge below:

[![Gitpod](https://gitpod.io/button/open-in-gitpod.svg)][1]

Instead, if you aim to test for different **`distros/releases`**, do:
1. Edit the file [`.gitpod.Dockerfile`](/.gitpod.Dockerfile) and create a new branch. In detail, you have to customize the [starting Docker image][2] as well as the [packages][3] to download.
2. Launch the corresponding Gitpod workspace from within the new branch. Don't click on the main badge but rather customize the [URL context][4]. To ease this operation, you may install the [Gitpod browser extension][5].


[1]: https://gitpod.io/#https://github.com/icub-tech-iit/test-packages-gitpod
[2]: https://github.com/icub-tech-iit/test-packages-gitpod/blob/master/.gitpod.Dockerfile#L1
[3]: https://github.com/icub-tech-iit/test-packages-gitpod/blob/master/.gitpod.Dockerfile#L30-L32
[4]: https://www.gitpod.io/docs/context-urls/#branch-context
[5]: https://www.gitpod.io/docs/browser-extension