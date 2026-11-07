---
icon: fontawesome/solid/chart-pie
---

# Making a PAL (Primary Asset Label)

## Making a Data Asset

??? "If this is your first time"
    I recommend you create a folder in "Content" named: `YourUserName_PAL` and placing all of your PALs there.

    For example, if I made this folder, I would name it: `Gamest23_PAL`

    ![](img/PALFolder.png)

Either Right-Click on an empty space, or click `+ ADD`

Then Search for `Data Asset` and create it by clicking on the result.

![](img/Data Asset Search.png)


Within the pop-up Search, type `Primary` and click `Primary Asset Label`

![](img/Primary Asset Label.png)

Name it whatever you wish, and open it by Double-Clicking on the new Asset.

The following fields need to be modified:

??? Priority
    This sets the load priority for assets, higher the number, higher the priority.

    For example: if `Mod1` had a priority of 3, and `Mod2` that replaces the same assets as `Mod1` had a priority of 4, Payday 3 will load `Mod2` assets instead of `Mod1`'s.

??? "Chunk ID"
    This field is to be set a number above zero, and to **not** conflict/share with other local PAL's Chunk ID. You don't have to worry with this conflicting with mods *outside* your project. This assigns the ID to the cooked assets and needs to be remembered later.

`Cook Rule` Needs to be set to `Always Cook`

`Is Runtime Label` Needs to be `Enabled`

`Include Redirectors` is not necessary to be `Enabled` or `Disabled` for the functionality of your mod.

## Explicit Assets

This is where your Wwise Events go.

In the Content Browser, go to the "WwiseAudio" folder and open the "Events" folder.

Either go folder by folder and find the Events :Wwise-event:. Or in the `Search Content` field, type "Event" and click `AK Audio Event`.

Select the Events :Wwise-event:. Either by clicking on one, then ++ctrl++ clicking the others. Or press ++ctrl+a++ to select everthing.

Then, click and drag them into the `Explicit Assets` field.

![](img/Explicit Assets.png)

You can now save the PAL by either doing `Save All` and `Save Selected`.

![](img/Save All.png) ![](img/Save Selected.png)

Or by clicking on this icon:

![](img/Save Icon.png)

----

[:material-package-variant-closed: Package Project](Package Project.md)