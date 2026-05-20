---
icon: material/music
---

[1]: https://gamest23.github.io/PD3WwiseAudioModding/First%20Time%20Setup/UE%20Project/
[3]: https://gamest23.github.io/PD3WwiseAudioModding/WwiseInfo/WwiseInfo/

## Work Unit Download

There is no Work Unit download for this guide.

## Event(s)

Go into the Events tab. The following image of Events[^3^][3] is required to be made, in order to replace the sound properly. Please recreate the image in its folder structure, and naming.

![ExampleImage](img/MainMenuMusicEvents.png)

We'll come back to this event later.

## Interactive Music Hierarchy

Go into the "Audio" tab and look for the "Interactive Music Hierarchy" folder.

In the Default Work Unit, make a Music Playlist Container[^3^][3] and name it after the name of the music you are using.

![example](img/Playlist%20Container%20Example.png)

## Output Bus

The output bus needs to be changed in order for proper play in-game.

With the Music Playlist Container[^3^][3] selected, find this field:

![outputbus](img/OutputBus.png)

Click on the 3 dots next to it, and navigate to:

Master-Mixer Hierarchy > Default Work Unit > Master Audio Bus > Main

![MusicOutput](img/MusicOutput.png)

Select Music and click OK

## Audio Importing

Importing audio is easy. From file explorer, select the (.wav) audio you want to use, and drag it onto the respective Container.

A window will open on import settings. Everything can be left on its default setting, and click "Import".

Once your audio is imported to their proper Containers, click on the Music Playlist Container[^3^][3].

## Playlist Sorting

You need to click and drag your imported Music Segments[^3^][3], into the Music Playlist Editor[^3^][3].

![ExampleGif](img/image13.gif)

The Container plays the audio in order from top to bottom by default. So go ahead and organize it if you have multiple audio files playing, like an intro and loop if you have them.

To the right side of the Music Segments[^3^][3] inside the editor is a "Loop Count". Pressing down from the value of "1" will make it loop indefinitely, don't worry about it not being able to stop as of right now.

You do need to at least make one of the Music Segments[^3^][3] loop indefinitely, to avoid it stopping when it runs out of runtime.

![Loop](img/ChangetheLoop.png)

You can theoretically use Transitions with the Playlist Container[^3^][3] here, but it's least likely you are going to use transitions anyway, UNLESS you have an intro and loop or generally multiple Music Segments used. If you want to know more about them, open this:

??? Transitions

    Transitions is the controlled behavior whenever the game changes states. Like when it goes from stealth to control, a transition is responsible of what it should do.

    Going into the Transitions tab, here you can either be creative with this, or do the fastest/lazy way.

    ![Tab](img/Transitions%20Tab.png)

    The transition that it comes with, is the default/fallback. Whenever there isn't a dedicated transition, it will use this instead.

    ![DefaultTransition](img/DefaultTransition.png)

    You can create more Transitions on the right side.

    ![Create](img/Create%20Transition.png)

    With new Transitions, you can select its source with the >>, which can either be a Container or Music Segment. And select a Destination.

    The different sections, do different actions. You can see this when having a Transition selected.

    ![Options](img/Sections.png)

    ## Transition Options

    ### Source

    `Exit Source at:` determines how it should stop the Source audio for the transition. Whether it should end it immediately, next bar, etc.

    There is also the option for it to fade-out when it stops the Source. **It must be configured for it to function the way you wish.**

    ### Transition Segment

    This is used if you want a specific Music Segment[^3^][3] to play in-between the Source and Destination. With it's own set of properties to change like fade-in and out.

    ### Destination

    `Jump to:` controls what Music Segment[^3^][3] to play inside the Music Playlist Container[^3^][3] in the Destination. **This is Disabled if a Music Segment[^3^][3] is selected for the Destination.**

    `Sync to:` is to control how the start of the Destination Music Segment[^3^][3] should be, compared to the current runtime of the playing Source Music Segment[^3^][3]

    There is also the option for it to fade-in when it starts the Destination. **It must be configured for it to function the way you wish.**

## Preview

To see your music in action, you can use the wwise player with the Music Playlist Container[^3^][3] selected.

![example](img/wwise%20player%20example%20generic.png)

## Events, again

Open the event that was created previously, a window like this should be open:

![ExampleImage](img/Event.png)

On the bottom left, there's an option to "Add >>". Click on it, and click "Browse Object..."

Then search for the Music Playlist Container[^3^][3] that you made.

Once you find it, select and press OK.

## Paking

Press ++ctrl+s++ to save, and open the Unreal Engine Project you downloaded in First Time Setup[^1^][1]

Proceed to "[Paking Your Mod](/PD3WwiseAudioModding/UE Paking/Generate Sound Data/)" on the left hand side of the page