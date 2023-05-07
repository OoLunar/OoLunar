# Lunar Starstrum
Website: https://forsaken-borders.net

Email: lunar@forsaken-borders.net

Discord: Lunar#9860

# About Me
I have a strong passion in entertaining others and making tools for convenience. With a recent interest in performance, I strive to write efficient and maintainable code. I absolutely enjoy working with infrastructure and keeping the toolchain centralized. I've used Linux for 4 years and have been using Docker for 2 years.

# Education
- Self taught for 5 years, working with mainly C#.
- I took a year long programming course in high school, which taught the basics of Java and OOP. I found the course to be of limited practical use and never wish to take it again.

# Projects
- [Cookie Clicker](https://github.com/OoLunar/CookieClicker): A simple cookie clicker game written in C#. It uses HTTP Interactions, Postgres, Remora, Serilog and GenHTTP. So far, it's been a great learning experience for me, as I've learned a lot about performance.
- [Tomoe](https://github.com/OoLunar/Tomoe): My Discord bot that I've been working on ever since I started programming. Though it's been through several stages, I'm currently rewriting it for the 5th time, focusing on performance, functionality and readability. Tomoe uses EFCore with targetted Postgres support, DSharpPlus, DSharpPlus.CommandAll, LiveChartsCore and Serilog.
- [DSharpPlus.CommandAll](https://github.com/OoLunar/DSharpPlus.CommandAll): A command framework for DSharpPlus. It combines DSharpPlus.CommandsNext and DSharpPlus.SlashCommands into a single command framework. The goal is to accept commands from both application commands and text commands using the same code base. While currently functional, it's still in development and is not ready for production use. The only explicit dependencies are DSharpPlus, Humanizer and Microsoft.Extensions.DependencyInjection.
- [DSharpPlus](https://github.com/DSharpPlus/DSharpPlus/): A Discord API wrapper for .NET. In April 2021, I was invited to join the DSharpPlus team as the lead dev. At the time, I was mainly focused on maintaining the library, though I took a more active role cleaning up some of the code, adding new features and making the community a safer place to be. While I no longer contribute as regularly, I still help out when I can.
- [GithubDockerRunner](https://github.com/OoLunar/GithubDockerRunner): This Dockerizes the Github Runner for a specific repository or organization, supporting both Github Runner updates and Docker inside of Docker. This is currently in use on my server, though I have no plans to add public support for it.
- [DSharpPlus-Doc-Bot](https://github.com/OoLunar/DSharpPlus-Doc-Bot): I did not write the master branch, that was done by [SubZero0](https://github.com/SubZero0), who modified their [Discord.NET DocBot](https://github.com/SubZero0/DiscordNet-Docs) to work with DSharpPlus. What I did write was the `rewrite/v2` and `rewrite/v3` branches, which use reflection to generate documentation from the loaded assemblies. I intend to continue working on this project and source gen the documentation using the Roslyn API, however I have not had the motivation to do so.

# Languages
- C# (5 years). I use C# to mainly focus on performance, readability and functionality. I've used it for a variety of projects including Discord bots, HTTP servers, and infrastructure tools. Additionally, I manually write my `.csproj` files to add functionality that Visual Studio or Rider doesn't easily expose (such as Tasks, Source Generators and Post Build Events).
- Rust (4-8 months). A great language, though I'll need to learn more about it before I can use it effectively.
- Bash (4 years). Used off and on again for various projects.

# Libraries
- `System.Reflection`: I've committed war crimes using reflection. Creating objects from attributes or marker interfaces allows me to generate functionality and prevent code duplication.
- `Serilog`: A logging library for .NET. I use this for all of my projects, as it's easy to use, has a lot of features and is very fast.
- `EFCore`: An ORM for .NET. When I require database support, I go to EFCore as it's LINQ support is very helpful for generating queries saving me time from writing them manually.
- `Npgsql`: A Postgres driver for .NET. When EFCore is too slow or doesn't have support for a specific feature, I use Npgsql directly. Npgsql allows me to prepare commands, pass data en masse and use Postgres specific features.
- `DSharpPlus`: A Discord API wrapper for .NET. I use this when I need to interact with the Discord API for a quick project, as it's very easy to use and has full API support.
- `Microsoft.Extensions.Configuration`: When I'm not writing a library, MSE.Configurations is my goto for loading configuration files, reading environment variables and parsing command line arguments. Additionally, when configuration files are modified, MSE.Configuration will automatically reload them.
- `Microsoft.Extensions.DependencyInjection`: A dependency injection library for .NET. Dependency injection is a great way to keep code clean and organized, and MSE.DI is a great library for it.
- `Humanizer`: When I must convert objects into something user friendly, Humanizer provides a lot of useful features that I use regularly.
- `Ulid`: Oh how I absolutely adore Ulid. It's a fantastic alternative to Guid as it's faster, provides the date it was created on (with millisecond precision!), is smaller in size and is lexographically sortable. I use this for all of my projects that require any sort of ids or unique idenfications.

# VPS Experience
- Familiar with Debian and Debian based distros.
- Daily drives Void Linux. I am somewhat familiar with the kernel filesystem API's (`/proc`, `/dev` and `/sys`). I have not looked into other distros such as Arch or CentOS because I am currently pleased with Void Linux.
- Intimate knowledge of Docker and Docker Compose.
- I've written Docker images from scratch for my own projects that I've programmed.
- I've setup a Wireguard VPN server using secure features such as pre-shared keys and a private DNS server ([dnscrypt](https://github.com/DNSCrypt/dnscrypt-proxy)). Using `iptables`, `10.13.13.0` is proxied to the server's `localhost`. Devices on the VPN can access other devices through their assigned peer address.
- I currently use Nginx and Lets-Encrypt to manage my HTTP server, as Nginx is fast and reliable without bloat while LetsEncrypt gives me an SSL for free which automatically renews itself bi-monthly through Cloudflare DNS propagation and cron jobs.
- I'm familiar with how DNS works and have successfully setup a mail server with both Postfix and Dovecot, though I now use [poste.io](https://poste.io/) through Docker for convenience and a lot less headache.
