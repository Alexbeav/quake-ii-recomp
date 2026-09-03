# Quake II validation receipt

## Scope

- Game: Quake II, USA, `SLUS-00757`
- Version: `0.1.0`
- Catalog ID: `quake-ii-psx`
- Release repository: `Alexbeav/quake-ii-recomp`
- Publication state: not published

## Frozen inputs

- The source disc identity is in `catalog_identity.json`.
- The required BIOS is a legal SCPH-1001 dump. OpenBIOS is not supported.
- The complete owned CUE has one data track and one audio track.
- Generated retail code, the game executable, the disc, and BIOS remain
  outside Git.

## Required release gates

The release candidate must pass generation, Release build, headless startup,
clean source package, payload, license, and clean-path checks. Alex must then
pass visible gameplay from the exact package.

## Local preparation evidence

- Studio audit: no required failure; two optional box-art warnings
- Code generation: 44 shards and 2,502 dispatch entries
- Full Release build: passed
- Hidden 25-second startup: frame and VBlank counts reached 3,657
- Fatal state: none
- Automatic or failed freeze dumps: none

The hidden test proves bounded startup progress. It does not prove gameplay,
input, audio, saves, multiplayer, or package installation.
