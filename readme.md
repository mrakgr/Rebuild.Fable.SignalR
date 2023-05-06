# Overview

Taken from the [Fable.SignalR repo](https://github.com/Shmew/Fable.SignalR) and updated to .NET 7.

It should be possible to import the project by linking to this Github repo directly. It hasn't been tested yet.

Don't forget to run `npm install @microsoft/signalr`.

If you want to use these packages in you own project add `git https://github.com/mrakgr/Rebuild.Fable.SignalR.git master Packages: /nupkgs/` to your `paket.dependencies` file.

Also, make sure to add the `Rebuild` prefix to the package names, eg. `Rebuild.Fable.SignalR` instead of `Fable.SignalR` otherwise it will try to get the old package from Nuget.

To pack the repo run:

```shell
dotnet pack --include-source
ls -r src/*.nupkg | mv -Destination nupkgs/ -Force
```