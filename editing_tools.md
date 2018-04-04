## brew
 - you may see an error like this:
 `xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun.`
 - possible solution: https://apple.stackexchange.com/questions/254380/macos-sierra-invalid-active-developer-path
   - `xcode-select --install`

## iterm2 with solarized
 - https://www.iterm2.com/
 - `brew cask install iterm2`
 - go to profiles --> default colors, select premade

## neovim
 - `brew install neovim`
 - `nvim` is the command to run it not `neovim`

## vim
 - there might be an error regarding missing if_lua if running neocomplete
 - make a frameworks dir and change ownership:
  `sudo mkdir /usr/local/Frameworks`
  `sudo chown ketho /usr/local/Frameworks `
  `brew upgrade vim --with-luajit`
 - to see vim options: `brew options vim`
   - i think it's `--with-client-server` that should enable clipboard support on os x / mac os
 - save a session with `:mksession ~/session.vim`
 - open a session with `vim -S ~/session.vim` or `:source ~/session.vim`

## sublime 3
 - `command + shift + p` to open command palette
 - package control installs: `command + shift + p` then `install package <name>`
 - nice packages:
   - JEDI https://github.com/srusskih/SublimeJEDI

