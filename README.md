# Hello Docker App (Visual Studio course)

ASP.NET Core sample targeting .NET 7. The source project, Dockerfile and Compose
configuration are retained; generated output is rebuilt locally.

## Build

With the matching .NET SDK installed:

```bash
dotnet restore hellodockerapp.sln
dotnet build hellodockerapp.sln
```

Or use the existing Docker Compose configuration in Visual Studio/Docker.

## Local configuration

Create your own registry publishing profile locally in Visual Studio. Personal
publish profiles, `.pubxml.user` credentials, `.vs`, `bin` and `obj` are ignored
and should not be committed. No registry credentials are required just to build.

Removing these files from the current branch does not erase prior Git history.
Review or rotate any previously used publishing credential as appropriate.
