<!---->

<div align="center">
  <h1 align="center">🔌  lsp-timeout.nvim</h2>
</div>

<!-- <img width="100%" src="doc/preview.png" /> -->
https://github.com/hinell/lsp-timeout.nvim/assets/8136158/92e30089-192f-4c75-8bec-85ca36a2c06c

<!-- Use badges from https://shields.io/badges/ -->
[![PayPal](https://img.shields.io/badge/-PayPal-880088?style=flat-square&logo=pay&logoColor=white&label=DONATE)](https://www.paypal.me/biteofpie)
[![License](https://img.shields.io/badge/FOSSIL-007744?style=flat-square&label=LICENSE)](https://github.com/hinell/fossil-license)

> _Nvim plugin for nvim-lspconfig: stop idle servers & restart upon focus; keep your RAM usage low_

## Overview

Some LSP servers are terribly inefficient at memory management and can
easily take up gigabytes of RAM MBs if left unattended (just like VS Code huh?!). 
This plugin prevents excessive memory usage by stopping and restarting LSP servers 
automatically upon gaining or loosing window focus, keeping neovim fast.


## ⚡Features

- Stop & start LSP servers upon demand
- Lower RAM usage by unsed Neovim system window

## 🔒Requirements

- [Neovim 0.7.2+](https://github.com/neovim/neovim/releases)
- [nvim-lspconfig](https://github.com/neovim/nvim-lspconfig)

## 📦 Installation

#### [packer.nvim](https://github.com/wbthomason/packer.nvim)
```lua
-- $HOME/.config/nvim/lua/user/init.lua
packer.setup(function(use)
    use({
         "hinell/lsp-timeout.nvim",
        requires={ "neovim/nvim-lspconfig" },
        setup = function()
            vim.g["lsp-timeout-config"] = {
                -- ...
            }
        end
    })
end)
```

#### [lazy.vim](https://github.com/folke/lazy.nvim)
```lua
require("lazy").setup(
    {
	"hinell/lsp-timeout.nvim",
	dependencies={ "neovim/nvim-lspconfig" }
    }
)
```

#### [vim-plug](https://github.com/junegunn/vim-plug)
``` vim
Plug "hinell/lsp-timeout.nvim"
```

<!-- ## 🚀 Usage -->
 

### [DOCUMENTATION]
### [CONTRIBUTING]
### [DEVELOPMENT]

[DOCUMENTATION]: doc/index.md 'Contribution instructions (see also source code files)'
[CONTRIBUTING]: CONTRIBUTING.md 'Contribution instructions (see also source code files)'
[DEVELOPMENT]: DEVELOPMENT.md 'Devloper documentation (see also source code files)'
[d]: #project

### SUPPORT DISCLAIMER
[ps]: #production-status--support 'Production use disclaimer & support info'

_NO GUARANTEES UNTIL PAID. This project is supported and provided AS IS. See also [LICENSE]._

[LICENSE]: LICENSE

----

September 26, 2023</br>
Copyright ©  - Alexander Davronov (a.k.a Hinell), et.al.</br>
