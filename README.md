# Recyclarr - Premade Configuration

[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/mattiaginoble/recyclarr-config/blob/main/LICENSE)
![Static Badge](https://img.shields.io/badge/Radarr%20Version%20-%20v4%20-%20orange?link=https%3A%2F%2Fgithub.com%2FRadarr%2FRadarr)
![Static Badge](https://img.shields.io/badge/Sonarr%20Version%20-%20v4%20-%20blue?link=https%3A%2F%2Fgithub.com%2FSonarr%2FSonarr)
[![GitHub release](https://img.shields.io/github/v/release/mattiaginoble/recyclarr-config.svg?color=green)
[![Github All Releases](https://img.shields.io/github/downloads/mattiaginoble/recyclarr-config/total.svg)]()
[![Support Server](https://img.shields.io/discord/492590071455940612.svg?color=7289da&label=TRaSH-Guides&logo=discord&style=flat-square)](https://discord.com/invite/Vau8dZ3)

This is the repository for premade Configuration for the [Recyclarr](https://github.com/recyclarr/recyclarr) command line application 
that will automatically synchronize recommended settings from the [TRaSH guides](https://trash-guides.info/) to your Sonarr/Radarr instances.

All Quality Profiles are present for every need.
You will only need to recreate the profiles on Sonarr and Radarr with the same name, and then synchronize with Recyclarr.
To specify the desired language to search with Sonarr and Radarr, add a CF dedicated for the language manually in the Quality Profiles.

## Features

This preamde config supports Radarr and Sonarr v4. The following information is synced to
these services from the TRaSH Guides. For a more detailed features list, see the [Features](https://recyclarr.dev/wiki/features) page.

- Recyclarr Configuration Template
- Quality Profiles, including qualities and quality groups
- Custom Formats, including scores (from guide or manual)
- Quality Definitions (file sizes)

## Installation

[Install Recyclarr](https://recyclarr.dev/wiki/installation/).

Download and open the premade configuration file from the this latest release. Update the [`base_url` and `api_key` properties](https://recyclarr.dev/wiki/yaml/config-reference/basic/), and place in your [application data directory](https://recyclarr.dev/wiki/file-structure/#appdata-directory)

If that doesn't work, try run `recyclarr config create` to create a starter **recyclarr.yml** file in the [application data directory](https://recyclarr.dev/wiki/file-structure/#appdata-directory) and overwrite with this premade file.
Remember to update the [`base_url` and `api_key` properties](https://recyclarr.dev/wiki/yaml/config-reference/basic/)

Run `recyclarr sync`, and all settings on Radarr and Sonarr will be loaded, these will be automatically updated whenever this command is run in the terminal.

It is important to create Quality Profiles in Radarr and Sonarr according to your needs among the following.

Quality Profiles for Sonarr:
[WEB-DL (1080p)](https://trash-guides.info/Sonarr/images/cf-profile-web1080.png)
[WEB-DL (2160p)](https://trash-guides.info/Sonarr/images/cf-profile-web2160.png)
[Remux-1080p - Anime](https://trash-guides.info/Sonarr/images/cfa-default-scoring.png)

Quality Profiles for Radarr:
[HD Bluray + WEB](https://trash-guides.info/Radarr/images/qp-bluray-webdl.png )
[UHD Bluray + WEB](https://trash-guides.info/Radarr/images/qp-uhd-bluray-webdl.png)
[Remux-1080p - Anime](https://trash-guides.info/Radarr/images/cfa-complete.png )
[Remux + WEB 1080p](https://trash-guides.info/Radarr/images/qp-uhd-bluray-webdl.png )
[Remux + WEB 2160p](https://trash-guides.info/Radarr/images/qp-remux-webdl-2160p.png)

### Read the Recyclarr Documentation

Main documentation is located in [the wiki](https://recyclarr.dev/wiki). Links provided below for
some main topics.

- [Command Line Reference](https://recyclarr.dev/wiki/cli/)
- [Configuration Reference](https://recyclarr.dev/wiki/yaml/config-reference)
- [Settings Reference](https://recyclarr.dev/wiki/yaml/settings-reference)
- [Troubleshooting](https://recyclarr.dev/wiki/troubleshooting/help)
