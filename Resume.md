# Lunar Starstrum
Website: https://forsaken-borders.net
Email: lunar@forsaken-borders.net
Discord: Lunar#9860

# Education
- Self taught for 4 years, working with mainly C#.
- I took a year long programming course in high school, which taught the basics of Java and OOP. I gained very little experience from it and never wish to take it again.

# Projects
- Tomoe: My Discord bot that I've been working on ever since I started programming. Though it's been through several stages, I'm currently rewriting it for the 5th time, focusing on performance, functionality and readability.
- DSharpPlus.CommandAll: A command framework for DSharpPlus. It combines DSharpPlus.CommandsNext and DSharpPlus.SlashCommands into a single command framework. The goal is to accept commands from both application commands and text commands using the same code base. While currently functional, it's still in development and is not ready for production use.
- DSharpPlus: A Discord API wrapper for .NET. In April 2021, I was invited to join the DSharpPlus team as the lead dev. At the time, I was mainly focused on maintaining the library, though I took a more active role cleaning up some of the code, adding new features and making the community a safer place to be. While I no longer contribute as regularly, I still help out when I can.
- CurseWatcher: A project that polls the CurseForge API and notifies a Discord channel when a mod or modpack is updated (through a webhook). This is very likely to no longer work as the CurseForge API has changed since I last worked on it.
- GithubDockerRunner: This Dockerizes the Github Runner for a specific repository or organization, supporting both Github Runner updates and Docker inside of Docker. This is currently in use on my server, though I have no plans to add public support for it.
- DSharpPlus-Doc-Bot: I did not write the master branch, that was done by https://github.com/SubZero0, who modified their [D.NET DocBot](https://github.com/SubZero0/DiscordNet-Docs) to work with DSharpPlus. What I did write was the `rewrite/v2` and `rewrite/v3` branches, which use reflection to generate documentation from the loaded assemblies. I intend to continue working on this project and source gen the documentation using the Roslyn API, however I have not had the motivation to do so.

# Languages
- C# (4 years). Most proficient.
- Java (2 years). Will require money in order for me to touch it again.
- Python (N/A). I can read it, but I can't write it easily.
- Rust (4-8 months). A great language, though I'll need to learn more about it before I can use it effectively.
- Bash (4 years). Used off and on again for various projects.

# VPS Experience
- Familiar with Debian and Debian based distros.
- Daily drives Void Linux. I am somewhat familiar with the kernel filesystem API's (`/proc`, `/dev` and `/sys`). I have not looked into other distros such as Arch or CentOS because I am currently pleased with Void Linux.
- Intimate knowledge of Docker and Docker Compose.
- I've written Docker images from scratch for my own projects that I've programmed.
- I've setup a Wireguard VPN server using secure features such as pre-shared keys and a private DNS server ([dnscrypt](https://github.com/DNSCrypt/dnscrypt-proxy)). Using `iptables`, `10.13.13.0` is proxied to the server's `localhost`. Devices on the VPN can access other devices through their assigned peer address.
- I currently use Nginx and Lets-Encrypt to manage my HTTP server, as Nginx is fast and reliable without bloat while LetsEncrypt gives me an SSL for free which automatically renews itself bi-monthly through Cloudflare DNS propagation and cron jobs.
- I'm familiar with how DNS works and have successfully setup a mail server with both Postfix and Dovecot, though I now use [poste.io](https://poste.io/) through Docker for convenience and a lot less headache.