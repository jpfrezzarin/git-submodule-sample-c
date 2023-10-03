# git submodules sample

A sample repository to shows the git submodule feature

The repositories connects like the diagram bellow:

```
sample-c --> sample-b --> sample-a
```
- The **sample-c** repository has a submodule, **sample-b**
- The **sample-b** repository has another submodule, **sample-a**

After clone, execute the following commands in terminal:

```sh
git submodule sync --recursive
```

This will syncronize the submodules URL with the same method used in root repository (ssh or https).

 - The ```--recursive``` flag is to syncronize the submodules recursively

After, execute the command bellow to update the submodule:

```sh
git submodule update --init --recursive
```

- The ```--init``` initializes the submodule if it wasn't initialized.

- The ```--recursive``` flag is to syncronize the submodules recursively