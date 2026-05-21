# edu-awesome

Educational / tutorial repository for [awesome WM](https://awesomewm.org/), a highly configurable Lua-driven dynamic window manager. Part of the `~/EDU/` learning series — a working awesome config dropped on top of a fresh Arch / Kiro install.

## What's in this repo

- `etc/skel/` — user-facing configs that land in `/etc/skel/` and propagate to new users (or can be copied into an existing `$HOME`).
- `setup.sh`, `up.sh`, `cleanup.sh` — standard EDU bash scaffold.

## Installation

### From `nemesis_repo` (recommended)

```ini
[nemesis_repo]
SigLevel = Never
Server = https://erikdubois.github.io/$repo/$arch
```

```bash
sudo pacman -Syu
sudo pacman -S edu-awesome
```

You'll also need awesome itself:

```bash
sudo pacman -S awesome
```

### Manual

```bash
git clone https://github.com/erikdubois/edu-awesome.git
cd edu-awesome
sudo cp -r etc/skel/. /etc/skel/
```

Existing users can copy the config into their own home:

```bash
cp -rT /etc/skel ~/
```

## Websites

Information : https://erikdubois.be

## Social Media

Youtube : https://www.youtube.com/erikdubois

## License

See [LICENSE](./LICENSE).
