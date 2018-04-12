# apertium-all

[Apertium][1] is a free/open-source platform for developing rule-based machine
translation systems.

This repository holds submodules to core tools, other tools, and all Apertium
language modules and pairs.

To clone this repository with all its submodules, run

    git clone --recurse-submodules --shallow-submodules --depth 1 git@github.com:apertium/apertium-all.git

(Change `--depth 1` to `--depth N` to get the last N commits.)

Most users should not commit directly to this repository. All Apertium
repositories with the topic `apertium-all` are automatically updated in this
repository as submodules.

However, changes can be made to submodules in this repository after cloning it.
To make a commit to each changed submodule:

    git submodule foreach 'git commit -a -m <message>'
    git submodule foreach 'git push'

More information about using Git is [on the wiki][2]. More information about the
submodules is in the READMEs of those repositories under https://github.com/apertium.

[1]: http://wiki.apertium.org/
[2]: http://wiki.apertium.org/wiki/Using_Git
