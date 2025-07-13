# XadrezPontoCom
## Authors

- [@Mr-Mewo](https://github.com/Mr-Mewo) - XadrezPontoCom's creator, possibly a SCSS adict.
- [@MrPent0](https://github.com/MrPent0) - Father of Aurora. She can definetly destroy that girl from Queen's Gambit.


## Description

-- Do I know how to properly make a .md file? noooo not at aalll! --\
-- Do I know how to write proper english? Also no --

Hey! This is XadrezPontoCom, a half baked and most definetly not a [chess.com](https://www.chess.com/) copycat! 

It was made by me and my friend as our final high school project. I'm responsable for XadrezPontoCom, and he is the one who made [Aurora](https://github.com/Mr-Mewo/Aurora-Chess-Engine), the chess engine that runs alongside the interface. 

This Aurora git is also manteined by me, but the project belongs to the other guy. Whenever he creates a git for Aurora, I'll delete mine and link to that instead.

If you wish for a documentation of the project, you can refer to [this project report](https://drive.google.com/file/d/1SxbhKAtDL9tG6zuIbnnB5541FsGkHUqO/view?usp=sharing), it explain the entire technicalities of both projects. It had to be printed and signed, it exists somewhere in our school library...\
And yes, it is in portuguese (Use Google translate as your heart desisres).
## installation

Clone the project

```bash
  git clone https://github.com/Mr-Mewo/Xadrez-Ponto-Com
  
  cd Xadrez-Ponto-Com
```

You will (of course) need [Rust](https://www.rust-lang.org/tools/install) to use work on this project.

wasm32 target install.

```bash
  rustup target add wasm32-unknown-unknown
```

Trunk installation.
More detailed explanation at [Trunk documentation](https://trunkrs.dev/guide/getting-started/index.html).

```bash
  cargo install --locked trunk
```

Tauri installation.
Refer to [this doc](https://v2.tauri.app/start/) for Tauri prerequisites and installation.

```bash
  cargo install tauri-cli --locked
```
## Run Locally

It only runs at localhost:8080 at the current moment. The backend is on :7878. \
One day will make a .json file for this.

Running XadrezPontoCom for web:

```bash
  cd ./Xadrez-Ponto-Com/frontend/
  trunk serve
```

For running as an application:

```bash
  cd ./Xadrez-Ponto-Com/src-tauri/
  (or at root)
  cd ./Xadrez-Ponto-Com/

  cargo tauri dev
```

The server that runs the engine (only the Aurora's .exe file is included):

```bash
  cd ./Xadrez-Ponto-Com/backend/
  cargo run
```

At root you can also find run-web.bat\
It starts a development server with trunk, and also starts the backend.