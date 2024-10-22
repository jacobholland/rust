FROM rust:slim-bullseye

RUN curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh

WORKDIR /usr/src/myapp

COPY guessing-game .

RUN cargo new --vcs none guessing-game

# ENTRYPOINT [ "rustc", "main.rs" ]

ENTRYPOINT ["tail", "-f", "/dev/null"]
