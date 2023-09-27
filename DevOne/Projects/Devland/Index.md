Devland is a social networks specially designed for developers, everything is open source and open to the public.

## How will it work?

- I'm thinking of hosting everything inside the user's repositories.
- Devland will be a repository itself, with sub modules to it's users repositories.
- Every change to the information inside the client will be a commit.
- The commit history will be accessible from within the clients.
- We will need an API to interact with the Git repositories, sending the information in the structure we define.
- I'm thinking of using either TOML or JSON as the information format.

## How will it look?

- The app will be panel based, panels will be moveable and resizable.
    
- The web app layout will be customizable, panels will be able to be arranged like the user wants to.
    
- Devland will have a extensibility model, users will be able to create modules for Devland.
    
- Modules will be presented as panels.
    
- There will be themes for the web client.
    
- People will be able to create their own third party clients.
    
   ![[Devland.png]]

## How will posts work?

- Posts will have attachments that will be viewable on click.

## How will code snippets work?

- People will be able to suggest code changes.

## What can you do?

- **Posts**
    - Share
        - Text
        - Code snippets
        - Links
        - Emoji
        - Pictures
        - Videos
        - #Hashtags
    - Interact
        - View
        - Comment
        - Save
        - Quote
        - Mark it as useful
        - View the log
    - Expand
        - Posts are expansible.
- **CLI & TUI**
    - Interface with Devland directly from the shell.
        - Make posts
        - View posts
        - Comment posts
        - Save posts
        - View the log

## What can’t you do on Devland?

- Send GIF
- Send stickers
- Be rude