# Sync-EZTools

A short, focused PowerShell script to automate ensuring that all instances of EZ Tools in a given path have updated ancillary files

## Use Case

If you download EZ Tools using [Get-ZimmermanTools.ps1](https://ericzimmerman.github.io/#!index.md), this is the script for you! Making sure your EZ Tools are updated is only half the battle. Did you know that EvtxECmd, RECmd, and SQLECmd rely on YAML files that help enhance the output in various ways? You need to keep those updated! This script will help automate that process! But first, you must download EZ Tools, similar to the following example:  
  
![Downloading EZ Tools](https://raw.githubusercontent.com/AndrewRathbun/Sync-EZTools/refs/heads/main/Media/dopus_75xoui6wcD.gif)

Next, run this script by passing the path where your instance of EZ Tools resides, similar to the following example:  
  
![Updating EZ Tools](https://raw.githubusercontent.com/AndrewRathbun/Sync-EZTools/refs/heads/main/Media/dopus_sX1UGxNUim.gif)

Once you do this, you've successfully updated your instance of EZ Tools! Notice how I passed the path that contains within ALL the EZ Tools I downloaded. That way, EvtxECmd, RECmd, and SQLECmd will be updated in each of the .NET 4, .NET 6, and .NET 9 versions that were downloaded using the `-NetVersion 0` parameter within `Get-ZimmermanTools.ps1`

## Feedback

Please create an Issue if you have any issues or feature requests! Happy updating!
