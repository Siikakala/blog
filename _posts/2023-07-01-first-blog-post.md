---
title: First!!!!
author: Mira Ojamo
tags: [Daily life]
cw: [Rambling]
---
This is mostly just for testing purposes - for now.

So, I configured automatic update of this blog when I commit new post - it is run on Github pages, deployed by Github actions and the different categories are
their own repositories, which are included as submodules and necessary files for Jekyll symlinked to correct places. So - as the actual posts are in their own
repos, I had to update the submodules separately, until now! Created another workflow to the master repo, which pulls latest versions of all submodules and
commits them to the repo, which then triggers the site update dpeloyment workflow. That update workflow is in turn triggered by submodule workflow through API.
Nice :3