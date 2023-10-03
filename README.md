# git submodules sample

A sample repository to shows the git submodule feature 

After clone, execute the following commands in terminal:

```sh
git submodule sync --recursive
```

This will syncronize the submodules URL with the same method used in root repository (ssh or https).

 - The ```--recursive``` flag is to syncronize the submodules recursively (if the submodules has another submodule 👌)

After, execute the command bellow to update the submodule:

```sh
git submodule update --init --recursive
```

- The ```--init``` initializes the submodule if it wasn't initialized.

- The ```--recursive``` flag is to syncronize the submodules recursively