---
layout: single
title: Dialog Audio
permalink: /docs/features/audio
toc: true
sidebar:
  nav: "docs"
---


Sometimes you just want to add some sound to your visual novel, to  make the reader feel the emotion of the scene even more or to hear the characters speak. For this purpose Visual Novel Machinery is using the Unreal Engine Audio System to allow you to add background music, sound effects, or voice overs.

![Audio System]({{ site.baseurl }}/assets/images/Audio/audio-in-action.png)
```
dialog.text -character=cube -emotion=Idle "While having a mute game is also great, sound can make everything so much better."
dialog.text -character=cube -emotion=Idle "For example, let's add some background music."
audio.play.bgm -id=background-music
dialog.text -character=cube -emotion=Idle "Isn't this relaxing."
dialog.text -character=cube -emotion=Idle "But enough of this."
audip.stop.bgm
dialog.text -character=cube -emotion=Idle "It is time that we flip the page to a new chapter."
audio.play.sfx -id=page-turn
dialog.text -character=cube -emotion=Idle "And now that we are on a new page, let me introduce myself."
audio.play.dialog.voiceover -id=hello-voice
dialog.text -character=cube -emotion=Idle "Hello."
dialog.text -character=cube -emotion=Idle "I am Cube."
dialog.end -nextdialog=start
```

## Background Music
To add background music you'll need to first import your audio files into the Unreal Engine. After this has been done, you'll need to add another entry to your Dialog Audio Definitions Data Table. Ensure that you specify the type in the Dialog Audio Definition as Background Music, otherwise the Background Audio Nodes will not find it. After all of that you can now play and stop the background music using the [Dialog Audio Play Background Music Node]({{ site.baseurl }}{% link docs/nodes-reference/audio-play-bgm.md %}) and [Dialog Audio Stop Background Music Node]({{ site.baseurl }}{% link docs/nodes-reference/audio-stop-bgm.md %}). Just remember that only one background music can ever be played at the same time.

## Sound Effect
To add sound effect you'll need to first import your audio files into the Unreal Engine. After this has been done, you'll need to add another entry to your Dialog Audio Definitions Data Table. Ensure that you specify the type in the Dialog Audio Definition as Sound Effect, otherwise the Background Audio Nodes will not find it. After all of that you can now play and stop the sound effect using the [Dialog Audio Play Sound Effect Node]({{ site.baseurl }}{% link docs/nodes-reference/audio-play-sfx.md %}) and [Dialog Audio Stop Sound Effect Node]({{ site.baseurl }}{% link docs/nodes-reference/audio-stop-sfx.md %}). Just remember that only one sound effect can ever be played at the same time.

## Voice Overs
For voice overs there are two ways they can be set up. But same as with the previous types you'll need to import your voice overs into the Unreal Engine first. 

After this you need to decide which way you prefer to use the voice overs. You can either add them as voice overs to the Character Definition of the character talking. You would then use the [Dialog Audio Play Character Voice Over Node]({{ site.baseurl }}{% link docs/nodes-reference/audio-play-character-voice-over.md %}) to play the voice over. 

Alternatively you can also save them to the Dialog Definition in which they appear. Then you would use the [Dialog Audio Play Dialog Voice Over Node]({{ site.baseurl }}{% link docs/nodes-reference/audio-play-dialog-voice-over.md %}).

To stop it before it is done you can use the [Dialog Audio Stop Voice Over Node]({{ site.baseurl }}{% link docs/nodes-reference/audio-stop-voice-over.md %}). This node doesn't differentiate between character or dialog voice over.

You can also play voice over lines directly with the [Dialog Text Node]({{ site.baseurl }}{% link docs/nodes-reference/dialog-text.md %}). You can setup the properties of the node to either use Dialog Voice Overs or Character Voice Overs. It all depends on how you set everything up.

![Dialog Text Audio Settings]({{ site.baseurl }}/assets/images/Audio/dialog-text-audio-settings.png)

It is also important to note that you don't have to decide on either Character Voice Overs or Dialog Voice Overs. You can use both ways at the same time. Just remember that only one voice over can ever be played at the same time.
