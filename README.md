# KodiSetupGuide

## How To Install Genesis Kodi Add-on

Settings
System -> File Manager -> Add: http://srp.nu (SuperRepo)

System -> Settings -> Add-ons -> Install from Zip File
SuperRepo -> helix (version name) -> repositories -> repository.superrepo.org.helix.repositories-latest.zip
Get Add-ons -> SuperRepo Repositories -> Add-on repository -> SuperRepo All [helix]

System -> Settings -> Add-ons -> Get Add-ons -> SuperRepo All [helix] -> press "C" -> Force refresh -> go inside -> Add-on repository -> lambda's Kodi Add-ons -> Install
Get Add-ons -> SuperRepo Repositories -> Add-on repository -> SuperRepo All [helix]

System -> Settings -> Add-ons -> Get Add-ons -> lambda Add-on repository -> press "C" -> Force refresh -> go inside -> Video Add-ons -> Genesis -> Install (there you have NBA On-demand as well!!!)

If force refresh doesn't work, try Videos -> Add-ons -> Get More... -> Genesis -> Install

Videos -> Add-ons -> Genesis -> press "C" -> Add-on settings -> set your preference

## How to tweak Kodi's buffer size

```console
cd /storage/.kodi/userdata
touch advancedsettings.xml
```

```xml
<advancedsettings>
  <network>
    <buffermode>1</buffermode>
    <cachemembuffersize>0</cachemembuffersize>
    <readbufferfactor>10</readbufferfactor>
    <curlclienttimeout>45</curlclienttimeout>
  </network>
  <video>
    <smallstepbackseconds>5</smallstepbackseconds>
    <usetimeseeking>true</usetimeseeking>
    <timeseekforward>30</timeseekforward>
    <timeseekbackward>-30</timeseekbackward>
    <timeseekforwardbig>600</timeseekforwardbig>
    <timeseekbackwardbig>-600</timeseekbackwardbig>
    <percentseekforward>2</percentseekforward>
    <percentseekbackward>-2</percentseekbackward>
    <percentseekforwardbig>10</percentseekforwardbig>
    <percentseekbackwardbig>-10</percentseekbackwardbig>
    <playcountminimumpercent>90</playcountminimumpercent>
  </video>
  <gui>
    <algorithmdirtyregions>3</algorithmdirtyregions>
    <nofliptimeout>0</nofliptimeout>
  </gui>
</advancedsettings>
```

## How To add fonts to Kodi
- **Android**: `Android/data/org.xbmc.kodi/files/.kodi/userdata/`
- **OpenELEC**: `/usr/share/kodi/media/Fonts`
