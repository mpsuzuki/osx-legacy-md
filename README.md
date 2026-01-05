md
==

# What is this?

This program "md" is picked from Apple
[adv_cmds-147.tar.gz][github_adv_cmds-147],
which has been available from their
[official github repository][github_adv_cmds].

[github_adv_cmds-147]: https://github.com/apple-oss-distributions/adv_cmds/archive/refs/tags/adv_cmds-147.tar.gz
[github_adv_cmds]: https://github.com/apple-oss-distributions/adv_cmds

# Why?

"md" is a legacy tool to do something like "makedepend",
and some old MacOSX software like cctools uses it.
It was written for the Mach project in CMU, and bundled
in NeXTSTEP, and succeeded by MacOSX, and removed at
MacOSX 10.7. Thus, the latest adv_cmds does not include
"md" anymore.

To simulate old developer environment, it is better to
have "md", but it is not easy find that "adv_cmds" is
the place to dig. Also, the source is written in K&R era,
the recent compiler would refuses it to compile without
the flag to permit the outdated coding styles.

So "md.c" is separated and tweaked for recent compiler.
