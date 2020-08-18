# Redlabs Game Launcher Data

This repository contains all of the necessary data for the Redlabs Game Launcher to retrieve info about the current available games.

## Usage

The file `games.json` contains all of the info for the available games.

Each game must have this associated information:
| Variable | Description |
|----------|------------ |
| title | The game title |
| description | The game description |
| tagline | The tagline of the game (one sentence description) |
| download-url | The URL to download the game files |
| exe | The name of the exe |
| file-size | The size of the file, in bytes |
| date-modified | The date modified in the format MMDDYYYY |
| version | The current version of the game. This is used to check if the client's game must be updated or not |

Each game must have a folder with the necessary images. The folder name is the same as the game title.
