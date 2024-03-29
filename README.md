Test Packages on Gitpod
=======================

A one-off disposable environment to test packages for the **`latest ubuntu`** release of our SW distros.

To get started, simply click on the badge below:

[![Gitpod](https://gitpod.io/button/open-in-gitpod.svg)][1]

Find out more on [YARP-enabled Gitpod workspaces][2].

Instead, if you aim to test against different **`distros/releases`**, do:
1. 📝 Edit the file [`.gitpod.Dockerfile`](/.gitpod.Dockerfile) and create a **`new branch`**. In detail, you have to fiddle with these [sections][3].
1. 🚀 Launch the corresponding Gitpod workspace from within the new branch. Don't click on the main badge but rather customize the [URL context][4]. To ease this operation, you may install the [Gitpod browser extension][5].
1. 🧹 Possibly, finish up by wiping out the branch.

### ⚠ How to flush the docker cache
As Docker relies on cached sections, you may still be using an old image when you've just updated a package to test. To invalidate the cache forcing Docker to build the relevant sections entirely again, apply the following workarounds:
- If you aim to build the whole image again, increase the variable [`INVALIDATE_DOCKER_CACHE_ALL`][6].
- If you've just fixed up the packages and aim to download and install them again, increase the variable [`INVALIDATE_DOCKER_CACHE_DL`][7].

[1]: https://gitpod.io/from-referrer
[2]: https://github.com/robotology/community/discussions/459
[3]: https://github.com/icub-tech-iit/test-packages-gitpod/blob/master/.gitpod.Dockerfile#L7-L11
[4]: https://www.gitpod.io/docs/context-urls/#branch-context
[5]: https://www.gitpod.io/docs/browser-extension
[6]: https://github.com/icub-tech-iit/test-packages-gitpod/blob/master/.gitpod.Dockerfile#L5
[7]: https://github.com/icub-tech-iit/test-packages-gitpod/blob/master/.gitpod.Dockerfile#L97
