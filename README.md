<p align="center">
  <br /><img
    width="400"
    src="https://raw.githubusercontent.com/starship/starship/master/media/logo.png"
    alt="Starship – Cross-shell prompt"
  />
</p>
<p align="center">
  <a href="https://github.com/starship/starship/actions"
    ><img
      src="https://github.com/starship/starship/workflows/Main%20workflow/badge.svg?branch=master&event=push"
      alt="GitHub Actions workflow status"
  /></a>
  <a href="https://crates.io/crates/starship"
    ><img src="https://img.shields.io/crates/v/starship" alt="Crates.io version"
  /></a>
  <a href="https://repology.org/project/starship/versions"
    ><img
      src="https://repology.org/badge/tiny-repos/starship.svg"
      alt="Packaging status"/></a
  ><br />
    <a href="https://discord.gg/8Jzqu3T"
    ><img
      src="https://img.shields.io/discord/567163873606500352?logo=discord"
      alt="Chat on Discord"
  /></a>
  <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
<a href="#contributors"><img src="https://img.shields.io/badge/all%20contributors-64-orange" alt="All Contributors"></a>
<!-- ALL-CONTRIBUTORS-BADGE:END -->
</p>

<h4 align="center">
  <br />
  <a href="https://starship.rs">Website</a>
  ·
  <a href="#-installation">Installation</a>
  ·
  <a href="https://starship.rs/config/">Configuration</a>
</h4>
<p align="center">
  <a href="https://github.com/starship/starship/blob/master/README.md"
    ><img height="20" src="https://raw.githubusercontent.com/starship/starship/master/media/flag-us.png" alt="English"
  /></a>
  &nbsp;
  <a href="https://github.com/starship/starship/blob/master/docs/ja-JP/guide/README.md"
    ><img height="20" src="https://raw.githubusercontent.com/starship/starship/master/media/flag-jp.png" alt="日本語"
  /></a>
  &nbsp;
  <a href="https://github.com/starship/starship/blob/master/docs/zh-TW/guide/README.md"
    ><img height="20" src="https://raw.githubusercontent.com/starship/starship/master/media/flag-tw.png" alt="繁體中文"
  /></a>
  &nbsp;
  <a href="https://translate.starship.rs/project/starship-prompt/zh-CN"
    ><img height="20" src="https://raw.githubusercontent.com/starship/starship/master/media/flag-cn.png" alt="简体中文"
  /></a>
  &nbsp;
  <a href="https://translate.starship.rs/project/starship-prompt/de"
    ><img height="20" src="https://raw.githubusercontent.com/starship/starship/master/media/flag-de.png" alt="Deutsch"
  /></a>
  &nbsp;
  <a href="https://translate.starship.rs/project/starship-prompt/es"
    ><img height="20" src="https://raw.githubusercontent.com/starship/starship/master/media/flag-es.png" alt="Español"
  /></a>
  &nbsp;
  <a href="https://translate.starship.rs/project/starship-prompt/fr"
    ><img height="20" src="https://raw.githubusercontent.com/starship/starship/master/media/flag-fr.png" alt="Français"
  /></a>
  &nbsp;
  <a href="https://translate.starship.rs/project/starship-prompt/ru"
    ><img height="20" src="https://raw.githubusercontent.com/starship/starship/master/media/flag-ru.png" alt="Русский"
  /></a>
</p>

<h1></h1>

<p align="center">
Starship is the minimal, blazing fast, and extremely customizable prompt for any shell!<br>
The prompt shows information you need while you're working, while staying sleek and out of the way.
<p>

<p align="center">
  <br>
  <img alt="Starship with iTerm2 and the Snazzy theme" src="https://raw.githubusercontent.com/starship/starship/master/media/demo.gif" width="80%">
  <br>
  <br>
</p>

## 🍬 Features

- Prompt character turns red if the last command exits with non-zero code
- Current Go version (`🐹`)
- Current Haskell version (`λ`)
- Current Java version(`☕`)
- Current Node.js version(`⬢`)
- Current PHP version (`🐘`)
- Current Python version (`🐍`)
- Current Ruby version (`💎`)
- Current Rust version (`🦀`)
- Current .NET version (`•NET`)
- Current version of package in current directory (`📦`)
  - npm (Node.js)
  - cargo (Rust)
  - poetry (Python)
  - composer (PHP)
- Current Git branch and rich repo status:
  - `=` — conflicting changes
  - `⇡` — ahead of remote branch
  - `⇣` — behind of remote branch
  - `⇕` — diverged changes
  - `?` — untracked changes
  - `$` — stashed changes
  - `!` — modified files
  - `+` — added files
  - `»` — renamed files
  - `✘` — deleted files
- Current Mercurial branch
- Current battery level and status
- `⇡` – charging
- `⇣` – discharging
- `•` – fully charged
- Indicator for jobs in the background (`✦`)
- Current Kubernetes Cluster and Namespace (`☸`)
- Current Amazon Web Services (AWS) profile (`☁️`)
- Execution time of the last command
- Custom environment variable value
- Nix-shell environment detection
- Current username if not the same as the logged-in user
- Optional current time in 12/24hr format

## 🚀 Installation

### Prerequisites

- A [Powerline font](https://github.com/powerline/fonts) installed and enabled in your terminal (for example, try [Fira Code](https://github.com/tonsky/FiraCode)).

### Getting Started

1. Install the **starship** binary:

   #### Install Latest Version

   ##### From prebuilt binary, with Shell:

   ```sh
   curl -fsSL https://starship.rs/install.sh | bash
   ```

   ##### From source on [crates.io](https://crates.io/):

   ```sh
   cargo install starship
   ```

   #### Install via Package Manager

   ##### With [Homebrew](https://brew.sh/):

   ```sh
   brew install starship
   ```

   ##### With [Scoop](https://scoop.sh):

   ```powershell
   scoop install starship
   ```

1. Add the init script to your shell's config file:

   #### Bash

   Add the following to the end of `~/.bashrc`:

   ```sh
   # ~/.bashrc

   eval "$(starship init bash)"
   ```

   #### Fish

   Add the following to the end of `~/.config/fish/config.fish`:

   ```sh
   # ~/.config/fish/config.fish

   starship init fish | source
   ```

   #### Zsh

   Add the following to the end of `~/.zshrc`:

   ```sh
   # ~/.zshrc

   eval "$(starship init zsh)"
   ```

   #### PowerShell

   Add the following to the end of `~\Documents\PowerShell\Microsoft.PowerShell_profile.ps1` (or `~/.config/powershell/Microsoft.PowerShell_profile.ps1` on -Nix):

   ```sh
   # ~\Documents\PowerShell\Profile.ps1

   Invoke-Expression (&starship init powershell)
   ```

   #### Ion

   Add the following to the end of `~/.config/ion/initrc`:

   ```sh
   # ~/.config/ion/initrc

   eval $(starship init ion)
   ```

## 🔧 Configuration

For details on how to configure Starship, check out our [documentation](https://starship.rs/config/).

## 🤝 Contributing

We are always looking for contributors of **all skill levels**! If you're looking to ease your way into the project, try out a [good first issue](https://github.com/starship/starship/labels/🌱%20good%20first%20issue).

### High Priority Needs

- 👩‍💼 **Product Manager**
  - We have a GitHub Project and many unorganized/unprioritized features, as well as ideas that haven't yet been made into issues. Starship needs someone to own the product direction!
- 👩‍🎨 **Designer**
  - Like making eye-catching websites? Excellent! We are looking to create a beautiful landing page showing off Starship in all its glory. Helping design for Starship's brand is a great opportunity to try out new ideas!
- 👩‍💻 **Rust Developer**
  - There is _a lot_ of low-hanging fruit when it comes to writing idiomatic Rust, designing effective Rust architecture, performance optimizations, cross-platform build optimizations, and more! I ([@matchai](https://github.com/matchai)) am a beginner to Rust. Come point us in the right direction!

If you are interested in helping contribute to starship, please take a look at our [Contributing Guide](https://github.com/starship/starship/blob/master/CONTRIBUTING.md). Also, feel free to drop into our [Discord server](https://discord.gg/8Jzqu3T) and say hi. 👋

### Contributors

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://twitter.com/matchai"><img src="https://avatars0.githubusercontent.com/u/4658208?v=4" width="100px;" alt=""/><br /><sub><b>Matan Kushner</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=matchai" title="Code">💻</a> <a href="#design-matchai" title="Design">🎨</a> <a href="#ideas-matchai" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-matchai" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-matchai" title="Maintenance">🚧</a> <a href="https://github.com/starship/starship/pulls?q=is%3Apr+reviewed-by%3Amatchai" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/starship/starship/commits?author=matchai" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://github.com/johnletey"><img src="https://avatars0.githubusercontent.com/u/30328854?v=4" width="100px;" alt=""/><br /><sub><b>John Letey</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=johnletey" title="Code">💻</a> <a href="#ideas-johnletey" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/starship/starship/pulls?q=is%3Apr+reviewed-by%3Ajohnletey" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/starship/starship/commits?author=johnletey" title="Tests">⚠️</a></td>
    <td align="center"><a href="http://timmulqueen.com"><img src="https://avatars1.githubusercontent.com/u/6132021?v=4" width="100px;" alt=""/><br /><sub><b>Tim Mulqueen</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=Multimo" title="Code">💻</a> <a href="#ideas-Multimo" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/starship/starship/pulls?q=is%3Apr+reviewed-by%3AMultimo" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/starship/starship/commits?author=Multimo" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://github.com/sirMerr"><img src="https://avatars2.githubusercontent.com/u/11183523?v=4" width="100px;" alt=""/><br /><sub><b>Tiffany Le-Nguyen</b></sub></a><br /><a href="#ideas-sirMerr" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-sirMerr" title="Maintenance">🚧</a> <a href="https://github.com/starship/starship/pulls?q=is%3Apr+reviewed-by%3AsirMerr" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/starship/starship/commits?author=sirMerr" title="Documentation">📖</a></td>
    <td align="center"><a href="https://about.snuggi.es"><img src="https://avatars0.githubusercontent.com/u/26250962?v=4" width="100px;" alt=""/><br /><sub><b>​Snuggle</b></sub></a><br /><a href="#design-Snuggle" title="Design">🎨</a> <a href="#ideas-Snuggle" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-Snuggle" title="Maintenance">🚧</a> <a href="https://github.com/starship/starship/pulls?q=is%3Apr+reviewed-by%3ASnuggle" title="Reviewed Pull Requests">👀</a></td>
    <td align="center"><a href="https://github.com/mehcode"><img src="https://avatars1.githubusercontent.com/u/753919?v=4" width="100px;" alt=""/><br /><sub><b>Ryan Leckey</b></sub></a><br /><a href="https://github.com/starship/starship/pulls?q=is%3Apr+reviewed-by%3Amehcode" title="Reviewed Pull Requests">👀</a></td>
    <td align="center"><a href="https://github.com/youssefhabri"><img src="https://avatars3.githubusercontent.com/u/1578005?v=4" width="100px;" alt=""/><br /><sub><b>Youssef Habri</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=youssefhabri" title="Code">💻</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/chipbuster"><img src="https://avatars2.githubusercontent.com/u/4605384?v=4" width="100px;" alt=""/><br /><sub><b>Kevin Song</b></sub></a><br /><a href="https://github.com/starship/starship/issues?q=author%3Achipbuster" title="Bug reports">🐛</a> <a href="https://github.com/starship/starship/commits?author=chipbuster" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=chipbuster" title="Documentation">📖</a> <a href="https://github.com/starship/starship/commits?author=chipbuster" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://andrewda.me"><img src="https://avatars1.githubusercontent.com/u/10191084?v=4" width="100px;" alt=""/><br /><sub><b>Andrew Dassonville</b></sub></a><br /><a href="https://github.com/starship/starship/issues?q=author%3Aandrewda" title="Bug reports">🐛</a> <a href="https://github.com/starship/starship/commits?author=andrewda" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/MaT1g3R"><img src="https://avatars1.githubusercontent.com/u/15258494?v=4" width="100px;" alt=""/><br /><sub><b>MaT1g3R</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=MaT1g3R" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=MaT1g3R" title="Documentation">📖</a> <a href="https://github.com/starship/starship/commits?author=MaT1g3R" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://github.com/AZanellato"><img src="https://avatars3.githubusercontent.com/u/30451287?v=4" width="100px;" alt=""/><br /><sub><b>André Zanellato</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=AZanellato" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=AZanellato" title="Documentation">📖</a> <a href="https://github.com/starship/starship/commits?author=AZanellato" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://saghm.com"><img src="https://avatars2.githubusercontent.com/u/5875560?v=4" width="100px;" alt=""/><br /><sub><b>Saghm Rossi</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=saghm" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=saghm" title="Documentation">📖</a> <a href="https://github.com/starship/starship/commits?author=saghm" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://medium.com/@cappyzawa"><img src="https://avatars3.githubusercontent.com/u/12455284?v=4" width="100px;" alt=""/><br /><sub><b>Shu Kutsuzawa</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=cappyzawa" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=cappyzawa" title="Documentation">📖</a> <a href="https://github.com/starship/starship/commits?author=cappyzawa" title="Tests">⚠️</a> <a href="#translation-cappyzawa" title="Translation">🌍</a></td>
    <td align="center"><a href="https://github.com/iamsauravsharma"><img src="https://avatars0.githubusercontent.com/u/38726015?v=4" width="100px;" alt=""/><br /><sub><b>Saurav Sharma</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=iamsauravsharma" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=iamsauravsharma" title="Documentation">📖</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/andytom"><img src="https://avatars1.githubusercontent.com/u/108836?v=4" width="100px;" alt=""/><br /><sub><b>Thomas O'Donnell</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=andytom" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=andytom" title="Tests">⚠️</a> <a href="https://github.com/starship/starship/commits?author=andytom" title="Documentation">📖</a> <a href="https://github.com/starship/starship/pulls?q=is%3Apr+reviewed-by%3Aandytom" title="Reviewed Pull Requests">👀</a></td>
    <td align="center"><a href="https://github.com/bbigras"><img src="https://avatars1.githubusercontent.com/u/24027?v=4" width="100px;" alt=""/><br /><sub><b>Bruno Bigras</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=bbigras" title="Code">💻</a> <a href="https://github.com/starship/starship/pulls?q=is%3Apr+reviewed-by%3Abbigras" title="Reviewed Pull Requests">👀</a></td>
    <td align="center"><a href="https://neilkistner.com/"><img src="https://avatars1.githubusercontent.com/u/186971?v=4" width="100px;" alt=""/><br /><sub><b>Neil Kistner</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=wyze" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=wyze" title="Tests">⚠️</a> <a href="https://github.com/starship/starship/pulls?q=is%3Apr+reviewed-by%3Awyze" title="Reviewed Pull Requests">👀</a></td>
    <td align="center"><a href="http://ca.linkedin.com/in/qstrahl"><img src="https://avatars3.githubusercontent.com/u/2235277?v=4" width="100px;" alt=""/><br /><sub><b>Quinn Strahl</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=qstrahl" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=qstrahl" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://github.com/tivervac"><img src="https://avatars2.githubusercontent.com/u/3389524?v=4" width="100px;" alt=""/><br /><sub><b>Titouan Vervack</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=tivervac" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=tivervac" title="Tests">⚠️</a></td>
    <td align="center"><a href="http://nosubstance.me"><img src="https://avatars1.githubusercontent.com/u/1269815?v=4" width="100px;" alt=""/><br /><sub><b>Francisco Lopes</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=oblitum" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/ahouts"><img src="https://avatars1.githubusercontent.com/u/16907671?v=4" width="100px;" alt=""/><br /><sub><b>Andrew Houts</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=ahouts" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=ahouts" title="Documentation">📖</a> <a href="https://github.com/starship/starship/commits?author=ahouts" title="Tests">⚠️</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/nickwb"><img src="https://avatars2.githubusercontent.com/u/594211?v=4" width="100px;" alt=""/><br /><sub><b>Nick Young</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=nickwb" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=nickwb" title="Documentation">📖</a> <a href="https://github.com/starship/starship/commits?author=nickwb" title="Tests">⚠️</a> <a href="https://github.com/starship/starship/pulls?q=is%3Apr+reviewed-by%3Anickwb" title="Reviewed Pull Requests">👀</a></td>
    <td align="center"><a href="https://github.com/g2p"><img src="https://avatars1.githubusercontent.com/u/61678?v=4" width="100px;" alt=""/><br /><sub><b>Gabriel de Perthuis</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=g2p" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/Hofer-Julian"><img src="https://avatars1.githubusercontent.com/u/30049909?v=4" width="100px;" alt=""/><br /><sub><b>Hofer-Julian</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=Hofer-Julian" title="Documentation">📖</a></td>
    <td align="center"><a href="http://blog.unhappychoice.com"><img src="https://avatars3.githubusercontent.com/u/5608948?v=4" width="100px;" alt=""/><br /><sub><b>Yuji Ueki</b></sub></a><br /><a href="#content-unhappychoice" title="Content">🖋</a> <a href="#translation-unhappychoice" title="Translation">🌍</a></td>
    <td align="center"><a href="https://github.com/heyrict"><img src="https://avatars3.githubusercontent.com/u/25698503?v=4" width="100px;" alt=""/><br /><sub><b>谢祯晖</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=heyrict" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=heyrict" title="Documentation">📖</a> <a href="#translation-heyrict" title="Translation">🌍</a> <a href="https://github.com/starship/starship/pulls?q=is%3Apr+reviewed-by%3Aheyrict" title="Reviewed Pull Requests">👀</a></td>
    <td align="center"><a href="https://twitter.com/bookun2851"><img src="https://avatars2.githubusercontent.com/u/10346162?v=4" width="100px;" alt=""/><br /><sub><b>Kutsuzawa Ryo</b></sub></a><br /><a href="https://github.com/starship/starship/pulls?q=is%3Apr+reviewed-by%3Abookun" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/starship/starship/commits?author=bookun" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=bookun" title="Tests">⚠️</a> <a href="#translation-bookun" title="Translation">🌍</a></td>
    <td align="center"><a href="https://github.com/hdevalke"><img src="https://avatars1.githubusercontent.com/u/2261239?v=4" width="100px;" alt=""/><br /><sub><b>hdevalke</b></sub></a><br /><a href="#ideas-hdevalke" title="Ideas, Planning, & Feedback">🤔</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/jakubclark"><img src="https://avatars0.githubusercontent.com/u/19486495?v=4" width="100px;" alt=""/><br /><sub><b>Kuba Clark</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=jakubclark" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=jakubclark" title="Documentation">📖</a> <a href="https://github.com/starship/starship/commits?author=jakubclark" title="Tests">⚠️</a></td>
    <td align="center"><a href="http://breax.org"><img src="https://avatars2.githubusercontent.com/u/862483?v=4" width="100px;" alt=""/><br /><sub><b>Gimbar</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=gimbar" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=gimbar" title="Tests">⚠️</a> <a href="https://github.com/starship/starship/commits?author=gimbar" title="Documentation">📖</a></td>
    <td align="center"><a href="http://tomhotston.net"><img src="https://avatars0.githubusercontent.com/u/22729355?v=4" width="100px;" alt=""/><br /><sub><b>Tom Hotston</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=TomHotston" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=TomHotston" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/bijancn"><img src="https://avatars3.githubusercontent.com/u/2117164?v=4" width="100px;" alt=""/><br /><sub><b>Bijan Chokoufe Nejad</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=bijancn" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=bijancn" title="Tests">⚠️</a> <a href="https://github.com/starship/starship/pulls?q=is%3Apr+reviewed-by%3Abijancn" title="Reviewed Pull Requests">👀</a></td>
    <td align="center"><a href="https://github.com/yuri1969"><img src="https://avatars3.githubusercontent.com/u/13468636?v=4" width="100px;" alt=""/><br /><sub><b>yuri</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=yuri1969" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=yuri1969" title="Documentation">📖</a> <a href="https://github.com/starship/starship/commits?author=yuri1969" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://github.com/TsubasaKawajiri"><img src="https://avatars2.githubusercontent.com/u/39114857?v=4" width="100px;" alt=""/><br /><sub><b>TsubasaKawajiri</b></sub></a><br /><a href="#translation-TsubasaKawajiri" title="Translation">🌍</a></td>
    <td align="center"><a href="https://github.com/qryxip"><img src="https://avatars2.githubusercontent.com/u/14125495?v=4" width="100px;" alt=""/><br /><sub><b>Ryo Yamashita</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=qryxip" title="Code">💻</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://pbzweihander.github.io"><img src="https://avatars2.githubusercontent.com/u/15262528?v=4" width="100px;" alt=""/><br /><sub><b>Thomas Lee</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=pbzweihander" title="Code">💻</a></td>
    <td align="center"><a href="https://pt2121.github.io"><img src="https://avatars0.githubusercontent.com/u/616399?v=4" width="100px;" alt=""/><br /><sub><b>(´⌣`ʃƪ)</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=pt2121" title="Code">💻</a></td>
    <td align="center"><a href="https://southcla.ws"><img src="https://avatars1.githubusercontent.com/u/1636971?v=4" width="100px;" alt=""/><br /><sub><b>Barnaby Keene</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=Southclaws" title="Code">💻</a></td>
    <td align="center"><a href="http://keawade.io/"><img src="https://avatars2.githubusercontent.com/u/7308850?v=4" width="100px;" alt=""/><br /><sub><b>Keith Wade</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=keawade" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=keawade" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://github.com/LukeAI"><img src="https://avatars3.githubusercontent.com/u/43993778?v=4" width="100px;" alt=""/><br /><sub><b>LukeAI</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=LukeAI" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/zekesonxx"><img src="https://avatars1.githubusercontent.com/u/965509?v=4" width="100px;" alt=""/><br /><sub><b>Zach Mertes</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=zekesonxx" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=zekesonxx" title="Documentation">📖</a> <a href="https://github.com/starship/starship/commits?author=zekesonxx" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://github.com/davidkna"><img src="https://avatars2.githubusercontent.com/u/835177?v=4" width="100px;" alt=""/><br /><sub><b>David Knaack</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=davidkna" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=davidkna" title="Documentation">📖</a> <a href="https://github.com/starship/starship/commits?author=davidkna" title="Tests">⚠️</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/CSumm"><img src="https://avatars1.githubusercontent.com/u/31711543?v=4" width="100px;" alt=""/><br /><sub><b>Carl Summers</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=CSumm" title="Documentation">📖</a></td>
    <td align="center"><a href="http://www.slmt.tw"><img src="https://avatars2.githubusercontent.com/u/6824412?v=4" width="100px;" alt=""/><br /><sub><b>Yushan Lin</b></sub></a><br /><a href="#translation-SLMT" title="Translation">🌍</a></td>
    <td align="center"><a href="https://weihanglo.tw"><img src="https://avatars2.githubusercontent.com/u/14314532?v=4" width="100px;" alt=""/><br /><sub><b>Weihang Lo</b></sub></a><br /><a href="#translation-weihanglo" title="Translation">🌍</a></td>
    <td align="center"><a href="https://github.com/pinshan"><img src="https://avatars0.githubusercontent.com/u/7709675?v=4" width="100px;" alt=""/><br /><sub><b>pinshan</b></sub></a><br /><a href="#translation-pinshan" title="Translation">🌍</a></td>
    <td align="center"><a href="https://github.com/brianlow"><img src="https://avatars2.githubusercontent.com/u/938138?v=4" width="100px;" alt=""/><br /><sub><b>Brian Low</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=brianlow" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=brianlow" title="Documentation">📖</a> <a href="https://github.com/starship/starship/commits?author=brianlow" title="Tests">⚠️</a></td>
    <td align="center"><a href="http://matiaskotlik.github.io"><img src="https://avatars2.githubusercontent.com/u/20362627?v=4" width="100px;" alt=""/><br /><sub><b>Matias Kotlik</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=matiaskotlik" title="Code">💻</a></td>
    <td align="center"><a href="https://marblenix.com"><img src="https://avatars0.githubusercontent.com/u/6401427?v=4" width="100px;" alt=""/><br /><sub><b>marblenix</b></sub></a><br /><a href="#infra-marblenix" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/starship/starship/commits?author=marblenix" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=marblenix" title="Tests">⚠️</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/weirongxu"><img src="https://avatars3.githubusercontent.com/u/1709861?v=4" width="100px;" alt=""/><br /><sub><b>Raidou</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=weirongxu" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=weirongxu" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://github.com/rpl"><img src="https://avatars1.githubusercontent.com/u/11484?v=4" width="100px;" alt=""/><br /><sub><b>Luca Greco</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=rpl" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=rpl" title="Documentation">📖</a> <a href="https://github.com/starship/starship/commits?author=rpl" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://lucar.in"><img src="https://avatars2.githubusercontent.com/u/6934358?v=4" width="100px;" alt=""/><br /><sub><b>Luca Rinaldi</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=lucarin91" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/REBELinBLUE"><img src="https://avatars1.githubusercontent.com/u/2143908?v=4" width="100px;" alt=""/><br /><sub><b>Stephen Ball</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=REBELinBLUE" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=REBELinBLUE" title="Tests">⚠️</a> <a href="https://github.com/starship/starship/commits?author=REBELinBLUE" title="Documentation">📖</a></td>
    <td align="center"><a href="http://about.houqp.me"><img src="https://avatars0.githubusercontent.com/u/670302?v=4" width="100px;" alt=""/><br /><sub><b>Qingping Hou</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=houqp" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=houqp" title="Documentation">📖</a> <a href="https://github.com/starship/starship/commits?author=houqp" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://github.com/wendorf"><img src="https://avatars3.githubusercontent.com/u/407342?v=4" width="100px;" alt=""/><br /><sub><b>Dan Wendorf</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=wendorf" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=wendorf" title="Tests">⚠️</a></td>
    <td align="center"><a href="http://popey.com/"><img src="https://avatars0.githubusercontent.com/u/1841272?v=4" width="100px;" alt=""/><br /><sub><b>Alan Pope</b></sub></a><br /><a href="#infra-popey" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/BuggStream"><img src="https://avatars1.githubusercontent.com/u/51194915?v=4" width="100px;" alt=""/><br /><sub><b>BuggStream</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=BuggStream" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=BuggStream" title="Documentation">📖</a></td>
    <td align="center"><a href="http://jonstodle.com"><img src="https://avatars1.githubusercontent.com/u/1719761?v=4" width="100px;" alt=""/><br /><sub><b>Jon Grythe Stødle</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=jonstodle" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=jonstodle" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://jasonet.co"><img src="https://avatars1.githubusercontent.com/u/10660468?v=4" width="100px;" alt=""/><br /><sub><b>Jason Etcovitch</b></sub></a><br /><a href="https://github.com/starship/starship/issues?q=author%3AJasonEtco" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://github.com/etiennemabille"><img src="https://avatars3.githubusercontent.com/u/11175343?v=4" width="100px;" alt=""/><br /><sub><b>Etienne Mabille</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=etiennemabille" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/Scotsguy"><img src="https://avatars3.githubusercontent.com/u/20385973?v=4" width="100px;" alt=""/><br /><sub><b>AppleTheGolden</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=Scotsguy" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=Scotsguy" title="Documentation">📖</a></td>
    <td align="center"><a href="http://sda.io"><img src="https://avatars1.githubusercontent.com/u/481987?v=4" width="100px;" alt=""/><br /><sub><b>Mike Sampson</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=mfs" title="Code">💻</a> <a href="https://github.com/starship/starship/commits?author=mfs" title="Documentation">📖</a> <a href="https://github.com/starship/starship/commits?author=mfs" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://sternentstehung.de"><img src="https://avatars3.githubusercontent.com/u/36575275?v=4" width="100px;" alt=""/><br /><sub><b>Dominik Braun</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=dominikbraun" title="Code">💻</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/dten"><img src="https://avatars0.githubusercontent.com/u/1019038?v=4" width="100px;" alt=""/><br /><sub><b>David Hewson</b></sub></a><br /><a href="https://github.com/starship/starship/commits?author=dten" title="Code">💻</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!

## 💭 Inspired By

Please check out these previous works that helped inspire the creation of starship. 🙏

- **[denysdovhan/spaceship-prompt](https://github.com/denysdovhan/spaceship-prompt)** - A ZSH prompt for astronauts.

- **[denysdovhan/robbyrussell-node](https://github.com/denysdovhan/robbyrussell-node)** - Cross-shell robbyrussell theme written in JavaScript.

- **[reujab/silver](https://github.com/reujab/silver)** - A cross-shell customizable powerline-like prompt with icons.

<p align="center">
    <br>
    <img width="100" src="https://raw.githubusercontent.com/starship/starship/master/media/icon.png" alt="Starship rocket icon">
</p>

## 📝 License

Copyright © 2019-present, [Starship Contributors](https://github.com/starship/starship/graphs/contributors).<br>
This project is [ISC](https://github.com/starship/starship/blob/master/LICENSE) licensed.
