# GamePanel — Game Server Repository

This repository hosts the **public game-server catalog** consumed by
[GamePanel](https://github.com/frogg-app/docker-game-servers). It contains a
single file, `game-servers.json`, which is a list of game-server definitions
(Docker image, default ports, environment variables, etc.).

It is published via **GitHub Pages**, and GamePanel's built-in
**"Official Repository"** points at that URL:

```
https://frogg-app.github.io/game-server-repository/game-servers.json
```

## Why this repo exists

The GamePanel application repo is private, so its files can't be fetched
anonymously. This public repo exists purely to serve the catalog to GamePanel
instances without requiring authentication.

## Adding or updating a game

Edit `game-servers.json` and open a pull request. Each entry follows the schema
already present in the file. Changes are published automatically by GitHub
Pages on merge to `main`, and GamePanel instances pick them up the next time
they refresh the Official Repository.