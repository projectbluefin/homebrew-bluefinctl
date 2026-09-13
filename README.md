# projectbluefin/bluefinctl — deprecated

> [!WARNING]
> **This tap is deprecated and archived. `bluefinctl` is retired and is no longer maintained.**

The `bluefinctl` formula in this tap has been marked `deprecate!` as of 2026-09-13. It will
still install and run so existing setups do not break abruptly, but Homebrew now prints a
deprecation warning, and no further releases will be published here.

## Replacement: chairlift

[`chairlift`](https://github.com/projectbluefin/chairlift) replaces `bluefinctl`.

It ships as a Homebrew **cask** from the `frostyard/tap` tap — not from a `projectbluefin`
tap. On current Bluefin images it is installed for you automatically, so most users need to
do nothing.

To install it by hand:

```sh
brew install --cask frostyard/tap/chairlift
```

## Cleaning up a manual install

If you tapped this repository and installed `bluefinctl` yourself, remove both:

```sh
brew uninstall bluefinctl
brew untap projectbluefin/bluefinctl
```

Bluefin images no longer ship `bluefinctl`, and systems that received it through the image
have it removed automatically on update — those users do not need to run anything.
