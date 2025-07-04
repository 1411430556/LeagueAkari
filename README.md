<div align="center">
  <div>
    <img
    src="https://github.com/LeagueAkari/LeagueAkari/raw/HEAD/pictures/logo.png"
    width="128"
    height="128"
    />
  </div>
  A League of Legends client toolkit based on the LCU API
</div>

<p align="center">
    <a href="https://github.com/LeagueAkari/LeagueAkari/releases"><img src="https://img.shields.io/github/release/LeagueAkari/LeagueAkari.svg?style=flat-square&maxAge=600" alt="Downloads"></a>
    <a href="https://github.com/LeagueAkari/LeagueAkari/releases">
    <img src="https://img.shields.io/github/downloads/LeagueAkari/LeagueAkari/total?style=flat&label=Downloads"></a>
    <a href="https://github.com/LeagueAkari/LeagueAkari/stargazers">
    <img src="https://img.shields.io/github/stars/LeagueAkari/LeagueAkari?style=flat&label=Stars">
  </a>
</p>

# 1. League Akari

A League of Legends client toolkit based on the LCU API.

## 1.2 Usage Instructions

Admin privileges are not required to run, but they enable additional features.

Supports most of the riot servers (not including Tencent).

## 1.3 Feedback Group

Fun places for casual chats, party setups, bug reports, and suggestions.

QQ Group: [301157623](https://qm.qq.com/q/F1Xv85etlm) or [543703181](https://qm.qq.com/q/jotnhHpG70) (Passcode: akari)

| 一群   | 二群 |
| :--------: | :------: |
| ![301157623](https://github.com/user-attachments/assets/2642c6a8-6162-459f-9faf-cb83b959c2c5) | ![543703181](https://github.com/user-attachments/assets/f418b2cd-f5e0-4613-93c5-f3e17cf00652) |

Telegram Group: [@LeagueAkari](https://t.me/leagueakari)

## 1.4 Beta Versions (.rabi)

"rabi" versions with features slated for the next release are periodically shared in the group chat.

# 2. Contributing to Development

Issues are inevitable; as a user, you can:

## 2.1 GitHub Issues

GitHub Issues is the primary channel for feedback. Please clearly describe your requirements, issues, or suggestions.

## 2.2 Contribute Code

Interested in the project? Feel free to contribute by submitting PRs and adding new features.

# 3. Build & Run

This section describes how to build League Akari from the source code.

## 3.1 Electron Main Program

```bash
yarn install
yarn dev
yarn build:win
```

## Private Packages

A valid GitHub PAT is required to install private packages.

`NODE_AUTH_TOKEN` must be set to the PAT value.

## 4. References

The development of **League Akari** has been greatly inspired by several outstanding open-source projects. These projects provided valuable insights and guidance for various modules of the software. We would like to extend our sincere appreciation to the authors and maintainers of the following resources:

| Project                                                                                            | Description                                                                          |
| -------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| [Pengu Loader](https://github.com/PenguLoader/PenguLoader)                                         | The ultimate JavaScript plugin loader, build your unmatched LoL Client.              |
| [League of Legends LCU and Riot Client API Docs](https://github.com/KebsCS/lcu-and-riotclient-api) | League of Legends LCU and Riot Client API Docs                                       |
| [Community Dragon](https://www.communitydragon.org/documentation/assets)                           | Resource management and asset documentation reference.                               |
| [Seraphine](https://github.com/Zzaphkiel/Seraphine)                                                | Provided integration approaches and insights into combining multiple tools.          |
| [fix-lcu-window](https://github.com/LeagueTavern/fix-lcu-window)                                   | Resolved the issue with abnormal window size of the League of Legends client.        |
| [Joi](https://github.com/watchingfun/Joi)                                                          | A League of Legends assistant. tool                                                  |
| [vscode-league-respawn-timer](https://github.com/Coooookies/vscode-league-respawn-timer)           | An extension to display League of Legends player respawn time in Visual Studio Code. |
| [LeaguePrank](https://github.com/LeagueTavern/LeaguePrank)                                         | Provided inspiration for playful and humorous features.                              |

# 5. Disclaimer

This software is a tool developed based on Riot's League Client Update (LCU) API. It does not use intrusive techniques and theoretically does not directly interfere with or modify game data. However, please be aware of potential compatibility issues or risks associated with game updates or anti-cheat systems.

The developer is not responsible for any consequences, such as account bans or data loss, resulting from the use of this software. Users are advised to fully understand the risks and take responsibility for their actions.

Additionally, **this application is not officially supported or endorsed by Riot Games**, all right reserved by Riot Games. Use it at your own risk, as it may violate the game's terms of service.

This disclaimer is intended to provide transparency and enable users to make informed decisions. Thank you for your understanding, and please ensure fair play in the gaming environment.

[![Star History Chart](https://api.star-history.com/svg?repos=LeagueAkari/LeagueAkari&type=Date)](https://star-history.com/#LeagueAkari/LeagueAkari&Date)
