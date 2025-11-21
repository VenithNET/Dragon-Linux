---
title: Copyright
date:  "2021-01-05T20:00:00+09:00"
draft: false
---

# Copyright policy

Dragon Linux is an open source project, and all contributions must follow the appropriate open source licenses.

These contribution rules are particularly important for code that is to be upstreamed into other projects, to maintain a clean paper trail of the licensing.

## Licensing

Code developed for Dragon Linux itself should be licensed under a permissive license that allows other projects to take advantage of the code without running into license compatibility problems. The specific licenses are subject to being decided on a case-by-case basis, but we will usually use a permissive license such as the MIT license.

Code developed for other open source projects must be licensed under that same project's license, and follow licensing/header/authorship conventions appropriate for that project. However, specific modules developed by Dragon Linux contributors (such as entire drivers or submodules) should be dual-licensed under a permissive license such as MIT, to ensure that they can be ported or reused within other projects.

For original code, we use [SPDX license identifiers](https://spdx.github.io/spdx-spec/v2.3/using-SPDX-short-identifiers-in-source-files/) to record the license of individual files in a concise way. Files should have header of this form (with whatever license information is appropriate):

```// SPDX-License-Identifier: GPL-2.0+ OR MIT```

No specific authors should be listed in source code files themselves, as this is hard to maintain and unlikely to remain accurate. For top-level and informational places where a copyright statement is needed, such as the MIT license text or "about" style dialogs, the code should be attributed to "The Dragon Linux Contributors".

We do not require contributors to accept any kind of CLA, nor do we require any kind of copyright assignment. You retain all copyright ownership of any code you write. These are merely conventions about how the origin of the code should be documented in version control and files.

## Attribution

Dragon Linux uses Git for managing source code, and the Git history serves as a record of authorship. The Git "Author" field should reflect the primary author of a change - if you commit a change authored by another person, you should ensure they are listed as the author. If a change is authored by multiple people, you should add one or more `Co-Developed-by: Foo Bar <foo@bar.com>` lines at the end of the commit message.

Non-Git releases of the software will be arranged to have an automatically generated authorship file containing a list of all Git contributors.

In order to certify the origin of contributions, all contributors are required to accept the Developer's Certificate of Origin 1.1:

> ## Developer’s Certificate of Origin 1.1
>
> By making a contribution to this project, I certify that:
>
> * The contribution was created in whole or in part by me and I have the right to submit it under the open source license indicated in the file; or
> * The contribution is based upon previous work that, to the best of my knowledge, is covered under an appropriate open source license and I have the right under that license to submit that work with modifications, whether created in whole or in part by me, under the same open source license (unless I am permitted to submit under a different license), as indicated in the file; or
> * The contribution was provided directly to me by some other person who certified (a), (b) or (c) and I have not modified it.
> * I understand and agree that this project and the contribution are public and that a record of the contribution (including all personal information I submit with it, including my sign-off) is maintained indefinitely and may be redistributed consistent with this project or the open source license(s) involved.

To certify this, add a line to the end of your Git commit message as follows:

```
Signed-off-by: Random J Developer <random@developer.example.org>
```

This can be automated by simply using `git commit -s`.

Real names are not required for authorship or sign-off info. We encourage people to use a name they are commonly known by (e.g. a name you commonly use to interact in similar spaces), as that helps establish trust.
