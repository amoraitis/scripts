# nuget-repo

A script that creates a container for a nuget feed based on [BaGet](https://loic-sharma.github.io/BaGet/).

The script creates a container which contains a nuget server, it adds the nuget feed to sources, and pushes the nupkgs to that feed.

## Setup

#### Prerequisites

[dotnet](https://dotnet.microsoft.com/) and [docker](https://www.docker.com/) already isntalled.

#### Steps

```
1. git clone https://github.com/amoraitis/scripts.git
2. cd scripts/nuget-repo
3. repos=(your project dirs here) // space separated dirsof containing a .csproj
4. ./add-repos ${repos[@]}
5. ./start-and-push YOUR_API_KEY_HERE
```

Instead of steps 3 and 4, you can just add line separated paths to the `repositories` file.