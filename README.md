<div align="center">

<a href="https://scii.io"><img src="https://raw.githubusercontent.com/sciiio/.github/main/profile/assets/hero.webp" width="100%" alt="scii: an ascii-native social network, terminal first. The terminal client's feed, its selection stepping down the posts while a reaction counts up."></a>

<a href="https://github.com/sciiio/scii-releases/releases/latest/download/scii-darwin-arm64"><img src="https://raw.githubusercontent.com/sciiio/.github/main/profile/assets/buttons/macos.svg" alt="download for macOS"></a>
<a href="https://github.com/sciiio/scii-releases/releases/latest/download/scii-linux-x64"><img src="https://raw.githubusercontent.com/sciiio/.github/main/profile/assets/buttons/linux.svg" alt="download for linux"></a>
<a href="https://scii.io/app"><img src="https://raw.githubusercontent.com/sciiio/.github/main/profile/assets/buttons/web.svg" alt="open the web app"></a>
<br>

**[scii.io](https://scii.io)** ·
**[Docs](https://scii.io/#docs)** ·
**[Web app](https://scii.io/app)** ·
**[All releases](https://github.com/sciiio/scii-releases/releases)**

</div>

<br>

This repository is where **scii**'s terminal client is published: one native binary for macOS (Apple
silicon) and one for Linux (x86-64), with a `SHA256SUMS` file, on every
[release](https://github.com/sciiio/scii-releases/releases). scii is a social network made of text:
posts, colors, avatars and images are all characters, in your terminal or at
[scii.io/app](https://scii.io/app).

## 📟 Install

<img src="https://raw.githubusercontent.com/sciiio/.github/main/profile/assets/install.webp" width="100%" alt="A terminal runs brew install sciiio/scii/scii, Homebrew installs it, and then runs scii to sign in and open the feed.">

**Homebrew** (macOS and Linux):

```sh
brew install sciiio/scii/scii
brew upgrade scii       # later, to update
```

**Or download** the binary for your platform from the
[latest release](https://github.com/sciiio/scii-releases/releases/latest), then:

```sh
shasum -a 256 -c SHA256SUMS --ignore-missing   # check it
chmod +x scii-darwin-arm64                     # or scii-linux-x64
mv scii-darwin-arm64 /usr/local/bin/scii
```

The macOS binary is signed with a Developer ID; `codesign -dv scii` shows it.

## 🚀 First run

```sh
scii            # sign in (scan the QR code with your phone) and open the feed
scii help       # every command
```

There are no passwords: you sign in with [Hypery](https://hypery.ai). In the feed, `j`/`k` move, enter
opens a thread, `n` posts and `1`–`8` react. The [docs](https://scii.io/#docs) cover every key, command
and setting.

<img src="https://raw.githubusercontent.com/sciiio/.github/main/profile/assets/features.webp" width="100%" alt="Six features, the selection stepping through them: images become ascii, color your words, made for the keyboard, tiny ascii reactions, themes from posts, and no passwords.">

## 🖼 Images become ascii

<img src="https://raw.githubusercontent.com/sciiio/.github/main/profile/assets/asciify.webp" width="100%" alt="A sunset picture beside scii's ascii render of it, the ramp control stepping through classic, blocks, shades and dense.">

Attach a png, jpeg, gif or webp and scii turns it into colored characters. Pick the ramp, the mode and
whether to keep color, and preview it before you post.

<br>

<sub>Releases are published here automatically from scii's source repository. The animations are made with
<a href="https://popcraft.app">PopCraft</a>; their source is in
<a href="https://github.com/sciiio/scii-popcraft">sciiio/scii-popcraft</a>.</sub>
