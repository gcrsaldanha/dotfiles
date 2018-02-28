Use symlink to link dotfiles from this folder to where they are expected to be:

```bash
# ln -sv <source> <target>
$ ln -sv git/.gitconfig ~/gitconfig
```
Note it will create a two-way data editing: if you edit the target, both files are affected.
