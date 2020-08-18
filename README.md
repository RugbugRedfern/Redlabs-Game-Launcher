# Redlabs Game Launcher Data

This repository contains all of the necessary data for the Redlabs Game Launcher to retrieve info about the current available games.

## Usage

The file `games.json` contains all of the info for the available games.

Each game must have this associated information:
```csharp
title // The game title
description // The description of the game
tagline // The tagline of the game (one sentence description)
download-url // The URL to download the game files
exe // The name of the exe
file-size // The size of the file, in bytes
date-modified // The date modified in the format MMDDYYYY
```
