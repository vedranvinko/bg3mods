# Baldur's Gate 3

Steam version on Linux

Download Ultimate Cheat Spells for Nexusmods, unpack under installation directory, into Mods dir (create if doesn't exist)

`/home/vedran/.steam/root/steamapps/compatdata/1086940/pfx/drive_c/users/steamuser/AppData/Local/Larian Studios/Baldur's Gate 3/Mods`

Download Script Extender - https://github.com/Norbyte/bg3se

Unpack `DWrite.dll` into `/home/vedran/.steam/root/steamapps/common/Baldurs Gate 3/bin`, and if you want to provide some configs for Script Extender, in the same directory create ScriptExtenderSettings.json file:

```json
{
  "CreateConsole": true
}
```

Find file `modsettings.lsx` under the path like above for mods - `/home/vedran/.steam/root/steamapps/compatdata/1086940/pfx/drive_c/users/steamuser/AppData/Local/Larian Studios/Baldur's Gate 3/PlayerProfiles/Public`

Into the file write the mod load order, using info form json file provided along the mod

```xml
<?xml version="1.0" encoding="UTF-8"?>
<save>
    <version major="4" minor="5" revision="0" build="400"/>
    <region id="ModuleSettings">
        <node id="root">
            <children>
                <node id="ModOrder">
                    <children>
                        <node id="Module">
                            <attribute id="UUID" value="28ac9ce2-2aba-8cda-b3b5-6e922f71b6b8" type="FixedString" />
                        </node>
                        <node id="Module">
                            <attribute id="UUID" value="8ec86e0e-3b6b-4d7a-b62f-821c4f1c4bd5" type="FixedString" />
                        </node>
                    </children>
                </node>
                <node id="Mods">
                    <children>
                        <node id="ModuleShortDesc">
                            <attribute id="Folder" type="LSString" value="GustavDev"/>
                            <attribute id="MD5" type="LSString" value=""/>
                            <attribute id="Name" type="LSString" value="GustavDev"/>
                            <attribute id="UUID" type="FixedString" value="28ac9ce2-2aba-8cda-b3b5-6e922f71b6b8"/>
                            <attribute id="Version64" type="int64" value="36028797018963968"/>
                        </node>
                        <node id="ModuleShortDesc">
                            <attribute id="Folder" type="LSString" value="Ultimate_Cheats"/>
                            <attribute id="MD5" type="LSString" value=""/>
                            <attribute id="Name" type="LSString" value="Ultimate Cheat Spell Collection"/>
                            <attribute id="UUID" type="FixedString" value="8ec86e0e-3b6b-4d7a-b62f-821c4f1c4bd5"/>
                            <attribute id="Version64" type="int64" value=""/>
                        </node>
                    </children>
                </node>
            </children>
        </node>
    </region>
</save>
```
