# Turborepo NPM Issue

This simple turborepo repository uses npm and nextjs. On the latest version of nextjs at the time of writing this (13.2.4), npm throws the error `error code ENOWORKSPACES error This command does not support workspaces.` while using it with turborepo.

This is happening for me on node version `18.15.0` and NPM version `9.6.1`.

I did some testing and found that the last version of nextjs that does not cause this issue is version `13.1.6`.

In the `apps` directory I setup two barebones nextjs starters. `latest` causes the issue and `older` does not.

Hopefully this is somewhat helpful to tracking down the issue. Thanks!
