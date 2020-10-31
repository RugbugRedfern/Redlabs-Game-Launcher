# Redlabs Game Launcher Data

This repository contains all of the necessary data for the Redlabs Game Launcher to retrieve info about the current available games.

## Usage

The file `master.json` contains a list of URLS to all of the available games.
Each URL must link to a JSON file containing the following information:

| Variable | Description | Example |
|----------|-------------|---------|
| title | The game title. | Adrift |
| description | The game description. | A low-poly survival game in a multi-dimensional realm. Collect resources and craft tools to fully automate your world! |
| tagline | The tagline of the game (one sentence description). | A survival game which takes place in a multi-dimensional realm. |
| color | The color of the game's page in the launcher. HEX format. | 53BA4D |
| downloadURL | The URL for the game download. | https://drive.google.com/file/d/1W-161CKM8fUfA97XPWNtIxOeCkeV93ce/view?usp=sharing |
| run | The file to run in order to launch the game. | Adrift.exe |
| fileSize | The size of the file, in megabytes. | 53 |
| screenshots | The image URLS for screenshots of the game as an array. Include https:// at the start of the URL if it is an external link. | "Screenshots/1.png", "Screenshots/2.png" |
| changelog | The changelog for the game as an array. | "version":"0.2.9", "date":"10302020", "title":"Launcher Release", "content":"Adrift has been released on the Redlabs Launcher!", "image":"Changelog/0.2.9.png" |

Each game must have a folder with the necessary images. The folder name is the same as the game title, with the spaces replaced by the character _.
