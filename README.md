# MicrobeTraceShiny

Easily launch [MicrobeTrace](https://github.com/CDCgov/MicrobeTrace) from R using Shiny

This repository was created for use by CDC programs to collaborate on public health surveillance related projects in support of the CDC Surveillance Strategy.  Github is not hosted by the CDC, but is used by CDC and its partners to share information and collaborate on software.

## Quick Start

Fire up R and...

```R
# install the package:
source("https://install-github.me/CDCGov/MicrobeTraceShiny")

MicrobeTraceShiny::launch_microbetrace()
```

And there you go!

The first time you run it, MicrobeTraceShiny will download all the files needed to run MicrobeTrace (roughly 12MB). Subsequent runs will require much less time (and bandwidth), since the files only need to be downloaded once.

## Full Documentation

```R
install_microbetrace(dev = FALSE, force = FALSE, useGit = FALSE)
```

Installs MicrobeTrace.

* `dev` - Should we install the dev branch? By default, installs the `master` branch. Use `dev = TRUE` to install the `dev` branch. Note that this is recommended, as the `master` branch presently includes a redirection rule that prevents MicrobeTraceShiny from working properly.
* `force` - Should we force the installation of MicrobeTrace, even if it appears to already be installed? Useful if you believe MicrobeTrace was not properly downloaded the first time (e.g. your connection was interrupted), or you want to update to the bleeding-edge version of MicrobeTrace.
* `useGit` - Should we attempt to get MicrobeTrace using `git`? If so, you must have `git` installed and available from PATH.

```R
launch_microbetrace(dev = FALSE, port)
```

Launches MicrobeTrace.

* `dev` - Should we use the dev branch? By default, runs the `master` branch. Use `dev = TRUE` to run the `dev` branch. Note that this is recommended, as the `master` branch presently includes a redirection rule that prevents MicrobeTraceShiny from working properly.
* `port` - From what port should MicrobeTrace be served? Defaults to Shiny's default port setting.

## Public Domain

This repository constitutes a work of the United States Government and is not
subject to domestic copyright protection under 17 USC § 105. This repository is in
the public domain within the United States, and copyright and related rights in
the work worldwide are waived through the [CC0 1.0 Universal public domain dedication](https://creativecommons.org/publicdomain/zero/1.0/).
All contributions to this repository will be released under the CC0 dedication. By
submitting a pull request you are agreeing to comply with this waiver of
copyright interest.

## License

The repository utilizes code licensed under the terms of the Apache Software
License and therefore is licensed under ASL v2 or later.

This source code in this repository is free: you can redistribute it and/or modify it under
the terms of the Apache Software License version 2, or (at your option) any
later version.

This source code in this repository is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE. See the Apache Software License for more details.

You should have received a copy of the Apache Software License along with this
program. If not, see http://www.apache.org/licenses/LICENSE-2.0.html

The source code forked from other open source projects will inherit its license.


## Privacy

This repository contains only non-sensitive, publicly available data and
information. All material and community participation is covered by the
Surveillance Platform [Disclaimer](https://github.com/CDCgov/template/blob/master/DISCLAIMER.md)
and [Code of Conduct](https://github.com/CDCgov/template/blob/master/code-of-conduct.md).
For more information about CDC's privacy policy, please visit [http://www.cdc.gov/privacy.html](http://www.cdc.gov/privacy.html).

## Contributing

Anyone is encouraged to contribute to the repository by [forking](https://help.github.com/articles/fork-a-repo)
and submitting a pull request. (If you are new to GitHub, you might start with a
[basic tutorial](https://help.github.com/articles/set-up-git).) By contributing
to this project, you grant a world-wide, royalty-free, perpetual, irrevocable,
non-exclusive, transferable license to all users under the terms of the
[Apache Software License v2](http://www.apache.org/licenses/LICENSE-2.0.html) or
later.

All comments, messages, pull requests, and other submissions received through
CDC including this GitHub page are subject to the [Presidential Records Act](http://www.archives.gov/about/laws/presidential-records.html)
and may be archived. Learn more at [http://www.cdc.gov/other/privacy.html](http://www.cdc.gov/other/privacy.html).

## Records
This repository is not a source of government records, but is a copy to increase
collaboration and collaborative potential. All government records will be
published through the [CDC web site](http://www.cdc.gov).

## Notices
Please refer to [CDC's Template Repository](https://github.com/CDCgov/template)
for more information about [contributing to this repository](https://github.com/CDCgov/template/blob/master/CONTRIBUTING.md),
[public domain notices and disclaimers](https://github.com/CDCgov/template/blob/master/DISCLAIMER.md),
and [code of conduct](https://github.com/CDCgov/template/blob/master/code-of-conduct.md).
