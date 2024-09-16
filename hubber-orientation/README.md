# Hubber Orientation Presentation

This directory contains the Hubber Orientation presentation. Follow the instructions below to set up and run the presentation.

This presentation is built using [slidev]().

## Prerequisites

Before you begin, ensure you have the following installed on your machine:

- [Node.js](https://nodejs.org/) (version 14.x or later)
- [npm](https://www.npmjs.com/) (version 6.x or later)

## Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/LadyKerr/gh-copilot-talk
    cd hubber-orientation
    ```

2. Install the dependencies:

    ```sh
    npm install
    ```

## Running the Presentation

To start the presentation, run the following command:

```sh
npm run dev
```

This will start a local server and open the presentation in your default browser.


## Additional Information

Feel free to update the introductory slides to include your image and information. The slides are located in the `slides.md`.


## Example Live Demo

NOTE: create a new repo locally and push to GitHub. See example [here](https://github.com/LadyKerr/copilot101-hubber) with PR [here](https://github.com/LadyKerr/copilot101-hubber/pull/2).

General demo:

## Installation
- open vscode and search for extension, install then auth
- click "your copilot" and show settings page
- back to editor, click on copilot icon at the bottom, show panel
- click chat icon in panel 

## IDE Demo
### Code Complete: 
example: validate email address
start typing to show code complete in action

```
import re

emailToVerify = 'hello@email.com'
match = re.match(r'[^@]+@[^@]+\.[^@]+', addressToVerify)

if match == None:
    print('Bad Syntax')
    raise ValueError('Bad Syntax')

```
show inline chat and also move on to chat

### Copilot Chat:
- use `/explain` to explain the code
- ask copilot: 
```
Create an impressive creative coding demo in python for 8,000 engineers at the developer week conference. This must be splashy and very very impressive to make people want to use GitHub Copilot. Can you help me and make something please?
```
- save code in a new file
- run with python <filename> (get an intentional error)
- error message in terminal, highlight and have copilot explain
- resolve error
- run again (wow)

- ask copilot chat: 

```
what else can I add to the game?
```

- implement suggestions
- ask: can I create wave sounds and save it as particle.wav?

- show slash commands, agents,
- /test . . . and all
- @github what can you do? how can I use git?
- #file:game.py generate a readme file for this game



## DOTCOM - Chat is Ent only currently
**On devrel repo**
- ask copilot: what are the most recent issues assigned to me?
- ask copilot: summarize this issue
- ask copilot: how do I create a markdown table?
- ask: where can I find the file about video editing?

- Push code and generate a summary
- highlight code and ask for explanations/help
- go to repo, highlight function, ask for help: https://github.com/LadyKerr/noseknows-demo

