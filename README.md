# Ian's kickstart.nvim

## Quickstart Kickstart

```bash
# Install
brew install neovim

# Pull config
git clone https://github.com/iandoesallthethings/kickstart.nvim.git "${XDG_CONFIG_HOME:-$HOME/.config}"/nvim

# Add an alias to edit the config
echo 'alias nvc="nvim ~/.config/nvim/init.lua"' >> .zshrc
# Or if you don't have zsh
echo 'alias nvc="nvim ~/.config/nvim/init.lua"' >> .bashrc

# Run it once to install everything
nvim
```

## Short takeaways

`init.lua` is the config. Edit that to change stuff.

`Lazy` is used for plugins. It runs automatically if it detects changes, but `:Lazy` works too.

`Telescope` is your new shortcut/navigator friend. `[Space]` then run whatever commands:

- `[F]ormat`
- `[/]` Fuzzy search current file
- `[Space]` (i.e. space twice) search open buffers
- `[S]earch [F]iles` in the dir you ran nvim from
- `[S]earch [H]elp` is an excellent fuzzy search of the neovim docs
- `[T]oggle comment by line` (This is mine)

There's also stuff like `treesitter` for finding references and `neo-tree` as a file browser and a bunch of other stuff, but I haven't really jumped into those yet.

## More docs

If you're reading this and you're not me and need more info, you really should be looking at the [original repo](https://github.com/nvim-lua/kickstart.nvim).

[The Only Video You Need to Get Started with Neovim](https://www.youtube.com/watch?v=m8C0Cq9Uv9o): Genuinely good walkthrough of the `:Tutor`, which I also recommend.

Also just run `:Tutor` and actually read it.
