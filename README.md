# Projects

> NOTES: 
> - These projects may come back to life at some point, but this is generally a single location for "not actively maintained projects, and likely will not be maintained for the foreseable future (or ever)"
> - These projects are subject to complete removable in the future (from HEAD, still will be tracked by git) 

## beyond-all-reason-autogroup-util

- Script used to help creating autogroup configuration for [Beyond All Reason](https://www.beyondallreason.info/)
- State - Dec 26, 2025:
    - Usable; would take a preset given from `beyond-all-reason-util-presets`, and produce a lua snippet that can be copy and pasted directly into the BYAR.lua config file to set unit autogroup presets
        - NOTE: relys on pulling a config file directly from BAR's source code, so may actually not work anymore until that is updated
    - All manual; no automatation for directly getting configuration autogroups into the correct directories
    - Worked correctly in game for skirmishes, had some issues with some units in the scenarios (could have been special units that caused it not to work)
- Likely to continue? No
    - Game's configuration may have changed since this last update, so may not work anymore
    - May pick back up if I get back into BAR, or if someone wants to take ownership, will transfer it over out of this archived repo

## beyond-all-reason-util-presets

- Directory with some of the input/output from the other BAR util repositories
- State - Dec 26, 2025:
    - Works; directly with `beyond-all-reason-autogroup-util`
- Likely to continue? No
    - See `beyond-all-reason-autogroup-util` for more info as to why

## portfollio-website

- Gatsby portfollio website built for self-hosted github runner
- State - Aug 21, 2025
    - Works; indended way for it to be used was by
        1. Having a private github repository that kept assets used for deployment/github web pages
        2. A self hosted github runner to host the dev and test versions of the docker images running the website
    - The overall goal of this project was to be setup in a way so that:
        1. Run both dev and test locally on a device on the network
        2. User A can check the dev version of the website on their phone or computer, and Dev A could do active development on the website so User A could see changes in realtime
        3. Test would be the final product ready to be shipped up to the CD repository to be served by github web pages
        4. **In general, be a highly configurable website to quickly stand up a portfolio website showcasing media** - The idea was to have most everything be in a config file, so that most could just do: download, modify, standup, deploy, modify, etc.
- Likely to continue? Possibly
    - Project has potential, and may be worked out completely in the future, but for now will remain in an archived state

## wg_client_config_generator

- Generates config ready for for mobile or desktop wireguard clients
- State - Aug 6, 2025
    - Not working; was essentially recreating https://github.com/h44z/wg-portal; use this project instead. Leaving this repo archived in case anyone wants to see the key and QR code generation logic.
- Likely to continue? No, archived as reference material for generating Wireguard keys using the cli with python