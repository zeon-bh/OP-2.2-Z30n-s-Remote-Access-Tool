
# Z30n's Remote Access Tool (v1.3)

A small mod for Stalker OP-2.2 or Cumulative Pack 2.2 that allows a player to access,view and search items in player created stashes remotely from any map in the zone using a simple GUI Interface. The GUI has support for English, Russian, Ukranian, French and Polish languages.

## Installation

**DISCLAIMER:** ALWAYS MAKE BACKUPS OF YOUR SAVE FILES AND GAMEDATA FOLDER(IF YOU HAVE PREVIOUSLY INSTALLED SOME MODS). THIS GAME IS NOTORIOUS FOR BREAKING YOUR SAVE FOR RANDOM REASONS, ESPECIALLY IF YOU ARE MODDING. YOU HAVE BEEN WARNED!!!

The Mod is safe to install in a new game or a pre-existing save file. Removing it mid playthrough is not recommended and will break your save file!!!

1. Download the zip file from the Github Repository.
2. Extract the files to your OP-2.2 game directory.
3. After extracting the zip files you should have a gamedata folder inside your OP-2.2 installed directory.

## File Conflicts
If you have any other previous mods installed in your OP-2.2 game directory, make sure to check which files are over written by this mod.

The files that MUST be overwritten are:

    1. binder_safe.script
    2. callback_use.script
    3. key_handlers.script
    4. portable_charger.ltx
    5. System.ltx

**THESE FILES SHOULD ABSOLUTELY MUST BE OVERWRITTEN OR THE MOD WILL NOT WORK!!!**

If you are using custom icons then you can ignore ui_icon_equipment.dds, but doing so will display a broken or missing icon for the Remote Access Tool. Other than the missing icon the item should work as intended.

If you are already using a modified System.ltx file and don't want to overwrite it, Find the line with the text [string_table]:

    [string_table]
    language	=
    font_prefix	=
    files = articles, ui, dialog_manager, cycle_task, treasure, ..... zstash_ui_msg

In the files section add zstash_ui_msg at the end and you are done.

## Remote Access Tool
To obtain the Remote Access Tool simply press **LEFT SHIFT + SEMICOLON(;)** to spawn the Remote Access Tool into your inventory. You should get a popup message.

Once you have obtained the Remote Access tool, you need to first add your stashes to the Remote Accesss Tool list to open them remotely.

v1.3 Remote Access Tool :
Opening the stashes using the Remote Access Tool requires you to have one of the following electric type artifacts:  

    - Sparkler - 3 Uses
    - Flash - 10 Uses
    - Moonlight - 25 Uses
    - Battery - 50 Uses

The number indicates how many times an artifact can be used to open a stash remotely. After using all the charges, the artifact will be removed from your inventory. If you have multiple different valid artifacts in your inventory, the artifact with the highest remaining uses will be prioritized first.

The artifact uses can be changed in the zstash_configs.script file by changing the value of ZSTASH_RAT_MULT variable. The number is a multiplier, For Eg. setting the value to 2, doubles the default artifact uses and so on.

Stolen Stashes cannot be opened with the Remote Access Tool. You must retrieve the stolen stash to get access to the stash remotely.

Stashes cannot be opened remotely during a blowout for balance and for safety reasons, to avoid data corruption on your save file.

#### A. Adding and renaming a stash using the Remote Access Tool
1. To add a new or an existing stash open the stash directly and you should see a popup dialog box. Enter the name of your stash into the dialog box. (If you leave it empty the stash name will be set to a default name based on which map the stash is placed). If you do not want to add the stash to the Remote Access tool and just want to open the stash then just hit Cancel and you should be able to access the stash normally.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/ibkvj488fq6vp31u6g200/RAT_ADD_01.jpg?rlkey=fc0sx5v6nld2lj8vmfynik2jb&st=9shazrvn&raw=1">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/47jkre6ye7oqujglkqs02/RAT_ADD_02.jpg?rlkey=4z652xrdkt24y4wg4rw88dbdw&st=7nr05ch3&raw=1">
</p>

2. Once you have entered the name and clicked OK, you should get a message informing you about the addition of new stash to the Remote Access Tool. You can open your PDA and check the stash map spot and verify the name and the status of the link to your Remote Access Tool.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/s1phbirzzrvu33kg1ifhm/RAT_ADD_03.jpg?rlkey=fxbalnzkdp2jqckjodw7uv9ni&st=c3ws8e1s&raw=1">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/munbiow2ykevgxaolff79/RAT_ADD_04.jpg?rlkey=exh79oe9zeua9bjt1ewd4m6wf&st=e4j328ru&raw=1">
</p>

3. You can now open your Remote Access Tool from your inventory to verify your stash is added to the Remote Accesss Tool list. You can now view the contents of your stash directly from the Remote Access Tool without using your PDA. Since this is a new stash the stash is indeed empty.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/f24mta2zu8lizfndiglt5/RAT_ADD_05.jpg?rlkey=uia96vyq133itpwrhmqcz63w5&st=k6b6nzgz&raw=1">
</p>

4. To Rename a stash click the Rename button and a dialog box should open with the current name of your selected stash. After Confirming the new name you should see the list updated with the new name of your stash.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/tj3hqwkxr1xdzxidh2yez/RAT_ADD_06.jpg?rlkey=1j3wleeb5b8oi8k3cuzirfwxo&st=ldn2g7qg&raw=1">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/3p4j781o2ir1oirt0p56x/RAT_ADD_07.jpg?rlkey=u7r47fxx0ajtq6rekq5e22kb7&st=u7fjh55q&raw=1">
</p>

5. Your stash map spot will also be updated with the new stash name.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/bqk1yz9778muxkwrx41pf/RAT_ADD_08.jpg?rlkey=0l4nm4r6pz95p6kf5vu0sy0no&st=pszpax0w&raw=1">
</p>

#### B. Preview stash contents using the Remote Access Tool

1. You can view the contents of your linked stashes without opening the stash. Viewing the stash contents does not consume Teleport artifact uses. Open your Remote Access Tool and select from the list of your linked stashes. After selecting the stash from the list a preview window should appear on the right displaying all the contents of your selected stash.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/9whozfh5vtjcg9zpzt42n/RAT_PREVIEW_01.jpg?rlkey=hmro2i56wqwof4mwjhkz0dndo&st=or2kdjdy&raw=1">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/x03uxdhnq66sf9k3uvrxc/RAT_PREVIEW_02.jpg?rlkey=2acgotdtc2el91sf5a9ywyewk&st=bicwavau&raw=1">
</p>

#### C. Searching for an item using Remote Access Tool
**(Update v1.3) The search works for both English and Russian Localization. For other languages, there is no option to input their respective text into the search box as this is an engine limitation and cannot be fixed with mods. Apologize for the inconvenience :(**

You can change the input language by pressing the text EN/RU located at the right end of the text box.
<p align="center">
  <img width="288" height="82" src="https://www.dropbox.com/scl/fi/sju7zsb7kggdwnkluolbc/RAT_RU_SEARCH.PNG?rlkey=oavqifgmnpfx8er3sdwqfl4uq&st=4vgu8si3&raw=1">
</p>
1. The Remote Access Tool has an in-built search function which allows you to search for an item from all of your linked stashes. Let's say you want to search for an item named dummy.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/y9ndfg66o3asn02ygwjb3/RAT_SEARCH_01.jpg?rlkey=yb1afw2yhyofgcn9kpq5ltpq6&st=tj1vt8rs&raw=1">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/vwfqmlzclb7uy23sdsm57/RAT_SEARCH_02.jpg?rlkey=1t7zcfa482itim9kgmfpahy58&st=7dn587dp&raw=1">
</p>

2. After clicking OK, you should get a preview window to the left showing you the results of all items matching the word 'dummy'.The Green text are the items from your search result and the yellow number is the total number of said item from all of your linked stashes. The following white text are the names of the stashes in which the item is stored and the quantity of said item.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/yxobsygcyjazefpx2ny3v/RAT_SEARCH_03.jpg?rlkey=aqsahzl286mgj3yftxtwkk595&st=onunzwuy&raw=1">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/26b2mccm29ukbhfw9k9ql/RAT_SEARCH_04.jpg?rlkey=lg85q0rdmozqoi8jlfkwe0ely&st=64phay7l&raw=1">
</p>

#### D. Removing Linked Stash from your Remote Access Tool

1. To Remove a linked stash from your Remote Access Tool, Remove the stash directly by using the "Take All" button in the stash UI. (This has to be done directly by interacting with the stash, you cannot remove the stash from the Remote Access Tool, you will get a warning if you try to do this.)

## Credits
AMK Team, OP-2.2 or Cumulative Pack 2.2<br/>
Translations done by Google Gemini 2.5 Pro Exp
