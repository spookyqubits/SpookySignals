# Spooky Signals · SpookyQubits

An independent collection of quantum communication games, alongside [Ghosts and Gates](https://spookyqubits.github.io/Ghosts_and_Gates/).

Collection URL: https://spookyqubits.github.io/SpookySignals/

## Games

- **Ghost Mail** — `games/ghost-mail/`. Solo Courier, Solo Spy, and Pass & Play for 2–3 people on one phone. Includes a Signal Lab, Calm Night and Noisy Night, an offline download, and a printable facilitator guide.
- **Ghost Relay** — `games/ghost-relay/`. A six-delivery teleportation mission for a Solo Operator or 2–3 people sharing Sender, Courier, and Receiver roles. Includes a limited classical-resend budget, conditional X/Z corrections, state replays, a Relay Lab, and a printable guide.

Each game has its own folder under `games/`. Additional games can be added without changing the collection's address. Only completed games appear in the library.

```text
SpookySignals/
  index.html                    collection home
  assets/                       shared artwork
  games/
    ghost-mail/
      index.html                game and Signal Lab
      guide.html                printable facilitator guide
    ghost-relay/
      index.html                teleportation game and Relay Lab
      guide.html                printable facilitator guide
  downloads/
    spooky-signals-classroom-kit.zip
```

## Run and host

This is a static website with no install step, external fonts, account system, or database. Serve this repository with `python3 -m http.server 8080` and open `http://localhost:8080`. Each game's self-contained HTML file can also run offline in a browser that supports local HTML files.

Publish from **Settings → Pages → Deploy from a branch → main → /(root)**. `.nojekyll` is included. The sibling Ghosts and Gates collection is hosted from its own repository.

## Sources and model scope

Ghost Mail implements preparation and measurement in the Z/X bases and an intercept-resend attack on Bennett and Brassard's BB84 protocol. It is a classical simulation, not a real quantum key exchange. Ghost Relay models ideal quantum teleportation with a shared Bell pair and two classical bits; channel faults and resend stamps are fictional teaching mechanics. Its replay distinguishes exact simulator state comparisons from evidence available on one unknown qubit. Scores are teaching rules, not security calculations. Sources, educational precedents, and model limits are in each game’s rules and guide. No measured learning-gain or first-of-its-kind claim is made.

Design and code prepared for SpookyQubits, 2 November 2026. Credits in linked materials remain with their authors.
