# Redlabs Game Launcher Data

This repository contains all of the necessary data for the Redlabs Game Launcher to retrieve info about the current available games.

## Usage

The file `games.json` contains all of the info for the available games.

Each game must have this associated information:
| Variable | Description |
|----------|------------ |
| title | The game title. |
| description | The game description. |
| tagline | The tagline of the game (one sentence description). |
| downloadURL | The URL to download the game files. |
| exe | The name of the exe. |
| folder | A custom name for the game folder incase the title includes special characters. Leave this blank for the folder name to default to the title with the spaces replaced by the character -. |
| fileSize | The size of the file, in bytes. |
| dateModified | The date modified in the format MMDDYYYY. |
| version | The current version of the game. This is used to check if the client's game must be updated or not. |
| externalLink | An optional link that will display above the description. |
| externalLinkInfo | The text which when clicked redirects to the external-link. If no external-link is specified, the text will simply be static. |
| screenshots | The image names of screenshots for the game. The screenshot images must be in a subfolder of the game folder called "Screenshots". In the case of an external link, the screenshots do not need to be in the screenshots folder. Elements of the screenshots array must have two elements, "name" (string) and "external" (bool). If the link is external, the name should be the URL of the image. If the link is internal, the name should just be the name of the image (with the extension). |

Each game must have a folder with the necessary images. The folder name is the same as the game title, with the spaces replaced by the character -.
