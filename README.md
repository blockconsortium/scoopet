<div align="left">
<h1 align="left"> 🍨 Scoopet 🍨 </h1>
<p>
<a>
<img src="https://ci.appveyor.com/api/projects/status/kbd3a9mibncbx8ds?svg=true"/>
</a>
<a>
<img src="https://img.shields.io/github/languages/code-size/integzz/scoopet.svg">
</a>
<a>
<img src="https://img.shields.io/github/repo-size/integzz/scoopet.svg">
</a>
<a>
<img src="https://img.shields.io/github/license/integzz/scoopet">
</a>
</p>
</div>

<p></p>

<div>
<p> A Bucket for the Best Windows Package Manager <a href="https://github.com/lukesampson/scoop"> Scoop </a>: Continuously Assisting in Academic Research.
</p>

<p align="left">
        <a href="README.md">English</a> | <a href="README_CN.md">简体中文</a>
</p>
</div>

For ones familiar with Scoop:

```
scoop bucket add scoopet https://github.com/integzz/scoopet
```

# :running: To Start

## :bike: Install Scoop

### :computer: Step 1: Enable remote policy in PowerShell

```powershell
Set-ExecutionPolicy RemoteSigned -scope CurrentUser
```

### :gear: Step 2: Customize your Scoop directory

```powershell
$env:SCOOP='Your_Scoop_Path'
[Environment]::SetEnvironmentVariable('SCOOP', $env:SCOOP, 'User')
```

> If you skip this step, all user installed Apps and Scoop itself will live in `c:/users/user_name/scoop`.

### :hammer: Step 3: Download and install Scoop

```powershell
Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://get.scoop.sh')
```

### :book: Step 4: Glance at quick-start by `scoop help`

For more information, please visit Scoop official site at 👉 https://scoop.sh/ 👈

## :car: Install Apps from this bucket

### :train: Step 1: Install Aria2 to accelerate downloading

```powershell
scoop install aria2
```

### :ticket: Step 2: Install Git to add new repositories

```powershell
scoop install git
```

if you are using VPN, you need to turn off aria2 before installing Apps

```powershell
scoop config aria2-enabled false
```

### :airplane: Step 3: Add this wonderful bucket and update, mo-mo-da~ :kiss:

```powershell
scoop bucket add scoopet https://github.com/integzz/scoopet
scoop update
```

### :rocket: Step 4: Install Apps

- Check the exact name of App by `scoop search`

```powershell
scoop search <app_name>
```

- Install Apps with assistance of plugin `scoop-completion`

```powershell
scoop install scoop-completion
scoop install <app_name>
```

> to use `scoop-completion`, just to hit `tab` after initial letters of App names

### :100: Step 5: List the official recommended buckets by `scoop bucket known`

```powershell
scoop bucket known

main [default]
extras [strongly recommended]
versions
nightlies
nirsoft
php
nerd-fonts
nonportable
java
games
jetbrains
```

## :m: Trivial

### Tweak with Parameters in Aria2

```powershell
scoop config aria2-enabled true
scoop config aria2-retry-wait 4
scoop config aria2-split 16
scoop config aria2-max-connection-per-server 16
scoop config aria2-min-split-size 4M
```

## :star: Summary

### Research Tools

|           App            | Auto-Update ? | Origenal ?                                                     |
| :----------------------: | :-----------: | -------------------------------------------------------------- |
|      CopyTranslator      |       √       | √                                                              |
|    GeoGebra-Portable     |       √       | √                                                              |
|          Gephi           |       √       | √                                                              |
|        Grammarly         |       √       | [Ash258](https://github.com/Ash258/Scoop-Ash258)-borrowed      |
|         Julia-cn         |       √       | √                                                              |
|         KingDraw         |       √       | √                                                              |
|          LyX-cn          |       √       | √                                                              |
|  Mathpix Snipping Tool   |       ×       | √                                                              |
|     Mendeley Desktop     |       √       | √                                                              |
|       Miniconda-cn       |       √       | [Extras](https://github.com/lukesampson/scoop-extras)-modified |
|         NetLogo          |       √       | √                                                              |
| Cytoscape [Debugging...] |       √       | √                                                              |

### Development Auxillary

|               App                | Auto-Update ? | Origenal ?                                                          |
| :------------------------------: | :-----------: | ------------------------------------------------------------------- |
|            Cyberduck             |       √       | √ migrated to [Extras](https://github.com/lukesampson/scoop-extras) |
|       Partition Assistant        |       ×       | √                                                                   |
|         scoop-completion         |       √       | [Ash258](https://github.com/Ash258/Scoop-Ash258)-borrowed           |
|              uTools              |       √       | [dorado](https://github.com/chawyehsu/dorado)-borrowed              |
| VirtualBox [with Extension Pack] |       √       | [Ash258](https://github.com/Ash258/Scoop-Ash258)-borrowed           |
|      VMware Workstation Pro      |       ×       | [Ash258](https://github.com/Ash258/Scoop-Ash258)-borrowed           |
|              WinGet              |       √       | [Ash258](https://github.com/Ash258/Scoop-Ash258)-borrowed           |

### Daily Work

|        App         | Auto-Update ? | Origenal ?                                                    |
| :----------------: | :-----------: | ------------------------------------------------------------- |
|    BaiduNetDisk    |       √       | √                                                             |
|   File Converter   |       √       | √                                                             |
|  Office Tool Plus  |       √       | √                                                             |
| VeraCrypt-Portable |       √       | [nickbudi](https://github.com/nickbudi/scoop-bucket)-borrowed |
|   Wise Care 365    |       √       | √                                                             |
| Wise Disk Cleaner  |       √       | [Ash258](https://github.com/Ash258/Scoop-Ash258)-borrowed     |
|     WPSOffice      |       √       | [dorado](https://github.com/chawyehsu/dorado)-borrowed        |

### Social & Entertainment

|        App        | Auto-Update ? | Origenal ?                                             |
| :---------------: | :-----------: | ------------------------------------------------------ |
|     DingTalk      |       √       | √                                                      |
|     LX Music      |       √       | √                                                      |
|      magnetW      |       √       | √                                                      |
|   NetEase Music   |       √       | [dorado](https://github.com/chawyehsu/dorado)-borrowed |
|      WeChat       |       √       | [dorado](https://github.com/chawyehsu/dorado)-borrowed |
|      You-Get      |       √       | √                                                      |
| QQ [Debugging...] |       √       | [dorado](https://github.com/chawyehsu/dorado)-borrowed |
