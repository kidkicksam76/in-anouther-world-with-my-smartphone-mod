# examplemod
yoooooo sam


hi wsp
the code im think of:

# This is an example mods.toml file. It contains the data relating to the loading mods.
# There are several mandatory fields (#mandatory), and many more that are optional (#optional).
# The overall format is standard TOML format, v0.5.0.
# Note that there are a couple of TOML lists in this file.
# Find more information on toml format here:  https://github.com/toml-lang/toml
# The name of the mod loader type to load - for regular FML @Mod mods it should be javafml
modLoader="javafml" #mandatory
# A version range to match for said mod loader - for regular FML @Mod it will be the forge version
loaderVersion="${36,}" #mandatory This is typically bumped every Minecraft version by Forge. See our download page for lists of versions.
# The license for you mod. This is mandatory metadata and allows for easier comprehension of your redistributive properties.
# Review your options at https://choosealicense.com/. All rights reserved is the default copyright stance, and is thus the default here.
license="${MIT}"
# A URL to refer people to when problems occur with this mod
#issueTrackerURL="https://change.me.to.your.issue.tracker.example.invalid/" #optional
# A list of mods - how many allowed here is determined by the individual mod loader
[[mods]] #mandatory
# The modid of the mod
modId="${reincartedwithasmartphonethemod}" #mandatory
# The version number of the mod
version="${1.0.0-alpha}" #mandatory
# A display name for the mod
displayName="${Reincarnated with a smarthphone The Mod}" #mandatory
# A URL to query for updates for this mod. See the JSON update specification https://docs.minecraftforge.net/en/latest/misc/updatechecker/
#updateJSONURL="https://change.me.example.invalid/updates.json" #optional
# A URL for the "homepage" for this mod, displayed in the mod UI
#displayURL="https://change.me.to.your.mods.homepage.example.invalid/" #optional
# A file name (in the root of the mod JAR) containing a logo for display
#logoFile="examplemod.png" #optional
# A text field displayed in the mod UI
#credits="" #optional
# A text field displayed in the mod UI
authors="${KidKick X Yoltexx}" #optional

# The description text for the mod (multi line!) (#mandatory)
description='''${This is an mod inspired by the anime Reincarted in a world with a smartphone}'''
# A dependency - use the . to indicate dependency for a specific modid. Dependencies are optional.
[[dependencies.${mod_id}]] #optional
# the modid of the dependency
modId="forge" #mandatory
# Does this dependency have to exist - if not, ordering below must be specified
mandatory=true #mandatory
# The version range of the dependency
versionRange="${36,37}" #mandatory
# An ordering relationship for the dependency - BEFORE or AFTER required if the dependency is not mandatory
# BEFORE - This mod is loaded BEFORE the dependency
# AFTER - This mod is loaded AFTER the dependency
ordering="NONE"
# Side this dependency is applied on - BOTH, CLIENT, or SERVER
side="BOTH"
# Here's another dependency
[[dependencies.${mod_id}]]
modId="minecraft"
mandatory=true
# This version range declares a minimum of the current minecraft version up to but not including the next major version
versionRange="${minecraft_version_range}"
ordering="NONE"
side="BOTH"


