
# Z30n's Remote Access Tool (v1.2.1)

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

Opening the stashes using the Remote Access Tool requires you to have a Teleport Artefact with enough minimum condition. The Teleport Uses in the top right indicates how many times you can open your stash remotely. By default a single Teleport artifact has around ~10 uses.

The Teleport uses can be changed in the zstash_configs.script file. You can set your prefered preset value.

Stolen Stashes cannot be opened with the Remote Access Tool. You must retrieve the stolen stash to get access to the stash remotely.

Stashes cannot be opened remotely during a blowout for balance and for safety reasons, to avoid data corruption on your save file.

#### A. Adding and renaming a stash using the Remote Access Tool
1. To add a new or an existing stash open the stash directly and you should see a popup dialog box. Enter the name of your stash into the dialog box. (If you leave it empty the stash name will be set to a default name based on which map the stash is placed). If you do not want to add the stash to the Remote Access tool and just want to open the stash then just hit Cancel and you should be able to access the stash normally.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/bs4vmv7ye5mwwvzspn5ez/RAT_add_rename_01.jpg?rlkey=9kbpu3s1f9oq7rytcpatheck0&st=0uscmxxq&raw=1">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/9i9r5xfgh205sx3v2fdcn/RAT_add_rename_02.jpg?rlkey=rcq8zx8yh67zkqg90pzapbt3v&st=jmtr6v8h&raw=1">
</p>

2. Once you have entered the name and clicked OK, you should get a message informing you about the addition of new stash to the Remote Access Tool. You can open your PDA and check the stash map spot and verify the name and the status of the link to your Remote Access Tool.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/8upf03pxa7fdikz8xq123/RAT_add_rename_03.jpg?rlkey=o5wtmd6eqdioiz5f3ovtzyh63&st=iynpv2xp&raw=1">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/h6te0md3e9qwoildqimpm/RAT_add_rename_04.jpg?rlkey=l8j4mhwp30dtlt9frvztwx05k&st=b18t7d11&raw=1">
</p>

3. You can now open your Remote Access Tool from your inventory to verify your stash is added to the Remote Accesss Tool list. You can now view the contents of your stash directly from the Remote Access Tool without using your PDA. Since this is a new stash the stash is indeed empty.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/cjcwc9votj367za8jbn09/RAT_add_rename_05.jpg?rlkey=cnx8bbr4gqplobcwv5x5a41bd&st=0h5v5qra&raw=1">
</p>

4. To Rename a stash click the Rename button and a dialog box should open with the current name of your selected stash. After Confirming the new name you should see the list updated with the new name of your stash.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/dc9hybxl2w93as7antngb/RAT_add_rename_08.jpg?rlkey=hec9dmrzr7o817vqjvz22kcg4&st=ljmse9tp&raw=1">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/yh8spdt9yzuidngl9bhng/RAT_add_rename_09.jpg?rlkey=y2gedzhpehb5m38v6ryjyxv3a&st=m9ztrdv5&raw=1">
</p>

5. Your stash map spot will also be updated with the new stash name.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/ooc20nknxss2gbgci0ihn/RAT_add_rename_10.jpg?rlkey=p36e5cjfy0gt82mbg9zohmbjo&st=xmaxv0vb&raw=1">
</p>

#### B. Preview stash contents using the Remote Access Tool

1. You can view the contents of your linked stashes without opening the stash. Viewing the stash contents does not consume Teleport artifact uses. Open your Remote Access Tool and select from the list of your linked stashes. After selecting the stash from the list a preview window should appear on the right displaying all the contents of your selected stash.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/3b6w3gixxroa4qgvdrt41/RAT_preview_01.jpg?rlkey=pmg40eigvteqj8l0uiw90zrky&st=kxg703rc&raw=1">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/kxvr8lcdxwnedpezdsiaq/RAT_preview_02.jpg?rlkey=8aa739zvit20koducmaq3811i&st=j29zdvw6&raw=1">
</p>

#### C. Searching for an item using Remote Access Tool
**As of v1.2 the search function only works properly if your game is running in English localization. Other localizations might have mixed or downright broken search results.**

1. The Remote Access Tool has an in-built search function which allows you to search for an item from all of your linked stashes. Let's say you want to search for an item named dummy.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/oanl2zbzdpj8teedraktm/RAT_search_01.jpg?rlkey=m77y06q4lgt1casa3nsow99vu&st=uq9nn89w&raw=1">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/kpwwgboczdc4kosab95r4/RAT_search_02.jpg?rlkey=mrlhgfuocrna6tfbuzwxf396s&st=tf0shl2w&raw=1">
</p>

2. After clicking OK, you should get a preview window to the left showing you the results of all items matching the word 'dummy'.The Green text are the items from your search result and the yellow number is the total number of said item from all of your linked stashes. The following white text are the names of the stashes in which the item is stored and the quantity of said item.

<p align="center">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/m7m1tufe60srtrw9pq3sw/RAT_search_03.jpg?rlkey=qy977ccnnj9k6k9e6rkqe7mke&st=oeh9i7ov&raw=1">
  <img width="426" height="240" src="https://www.dropbox.com/scl/fi/olh2qryw3nc5bm5b3ipq4/RAT_search_04.jpg?rlkey=9qa4mklm48xl4gox5gdl3zclv&st=p6mv7fkf&raw=1">
</p>

#### D. Removing Linked Stash from your Remote Access Tool

1. To Remove a linked stash from your Remote Access Tool, Remove the stash directly by using the "Take All" button in the stash UI. (This has to be done directly by interacting with the stash, you cannot remove the stash from the Remote Access Tool, you will get a warning if you try to do this.)

## Credits
AMK Team, OP-2.2 or Cumulative Pack 2.2<br/>
Translations done by Google Gemini 2.5 Pro Exp
