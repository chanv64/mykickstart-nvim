install kickstart nvim from 


modify init.lua to enable neo-tree
enable pyright
if black doesn't install read this
https://github.com/williamboman/mason.nvim/issues/1537

resolved by 
--
I also encountered a similar problem, which I resolved after installing 'python3-venv'

sudo apt install -y python3-venv``

starship
see this video
https://www.youtube.com/watch?v=ZbgulVriTPE&t=496s
copy starship.toml from DT
git clone https://gitlab.com/dwt1/dotfiles.git
install wezterm from 
sudo apt install wezterm - linux
for windows download from https://wezfurlong.org/wezterm/index.html
here's a good video to learn wezterm feature from https://www.youtube.com/watch?v=TTgQV21X0SQ&t=45s
get wezterm.lua config file from my dotfiles
or here is my current dotfiles for windows running wsl

---------------
local wezterm = require 'wezterm'

local config = {}
if wezterm.config_builder then
    config = wezterm.config_builder()
end
  
-- change config now
config.default_domain = 'WSL:Ubuntu-24.04'

initial_cols = 150
initial_rows = 100

config.font = wezterm.font 'JetBrainsMono NF'
config.font_size = 12

config.window_decorations = "RESIZE"
config.window_background_opacity = 0.95

-- For example, changing the color scheme:
config.color_scheme = 'Catppuccin Mocha'

return config
-----------



