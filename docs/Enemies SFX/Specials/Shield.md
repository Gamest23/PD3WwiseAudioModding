---
icon: material/shield
---

[1]: https://gamest23.github.io/PD3WwiseAudioModding/First%20Time%20Setup/UE%20Project/
[3]: https://gamest23.github.io/PD3WwiseAudioModding/WwiseInfo/WwiseInfo/

## Work Unit Download

Download this Work Unit:

[Shield SFX.wwu](Downloads/Shield%20SFX.wwu)

Open the project's directory and locate the "Actor-Mixer Hierarchy" folder. You want to place the downloaded Work Unit inside this folder.

![ExampleImage](img/Project%20Explorer.png)

Now open the Wwise Project. If the Project was already opened, it may prompt to refresh/restart the app.

## Event(s)

Go into the Events tab. The following image of Events[^3^][3] is required* to be made, in order to replace the sound properly. You don't have to make every event if you don't want to replace the other SFXs listed. Still, please recreate the image in its folder structure, and naming.

![ExampleImage](img/Shield%20SFX%20Events.png)

`NPC_S_Barge`

`npc_shield_dink`

`npc_shield_peephole_break`

We'll come back to these events later.

Now go into the Audio tab, and find the "Actor-Mixer Hierarchy" section. 

Under the section should be the Work Unit you imported previously. It'll contain the containers that you import your audio (.wav) files into.

Due to how Wwise handles imports, there are 2 settings that need to be applied for the audio to both work and sound good.

We're editing these Containers:

![ShieldSFXContainers](img/Shield%20SFX%20Containers.png)

## Output Bus

The first field that needs to be changed is the Output Bus

![outputbus](img/OutputBus.png)

Click on the 3 dots next to it, and navigate to:

Master-Mixer Hierarchy > Default Work Unit > Master Audio Bus > Main > VO > VO_NPC

![Exampleimage](img/NPC_System%20Bus.png)

Select NPC_System and click OK

## Global Obstruction

Next, go into the RTPC tab in the Container Property Editor

![Exampleimage](img/RTPC.png)

This tab will be responsible how much the audio will lower when it comes to walls, doors, and floors being in the way.

Due to how much this is up to you, this is a separate page entirely that can be [opened here](https://gamest23.github.io/PD3WwiseAudioModding/RTPC/RTPC/).

## Audio Importing

Importing audio is easy. From file explorer, select the audio you want to use, and drag it onto the respective Container.

A window will open on import settings, for this you want to import it as a ==Sound SFX==. Everything else can be left on its default setting.

![ExampleImage](img/ImportExample.gif)

If you want a preview of what to expect, Wwise has controls to play, pause, and stop the currently selected container/audio.

![Player](img/Play%20Controls.png)

Once you're happy with your work, go back to the Events tab.

## Events, again

Open the events that were created previously, a window like this should be open:

![ExampleImage](img/Event.png)

On the bottom left, there's an option to "Add >>". Click on it, and click "Browse Object..."

Then search for the Container[^3^][3] that you want to play, whenever this event is triggered.

Once you find it, select and press OK.

Go ahead and do this to the other potential events, unless you have another container to play for it.

## Paking

Press ++ctrl+s++ to save, and open the Unreal Engine Project you downloaded in First Time Setup[^1^][1]

Proceed to "[Paking Your Mod](https://gamest23.github.io/PD3WwiseAudioModding/UE%20Paking/Generate%20Sound%20Data/)" on the left hand side of the page