**_Hopefully, you will find the answer here!_**
***
### Q: Are you the developer of uYouPlus?
- I'm just a guy who put all the tweaks which are used in uYouPlus into a YouTube IPA. Anyone can do that if they want to (see [Building - Wiki](https://github.com/qnblackcat/uYouPlus/wiki/Building)). 
- **In short**: _I'm not the developer of uYouPlus. All the developers in [Credits](https://github.com/qnblackcat/uYouPlus#credits) are the developer of uYouPlus._

***
### Q: I got the IPA. How do I install uYouPlus?
❖ There are many tools to sideload IPA to your phone. AltStore and Sideloadly are recommended. See [Installation - Wiki](https://github.com/qnblackcat/uYouPlus/wiki/Installation) for more info. Of course, there are other alternatives, but I only cover AltStore and Sideloadly. 

***
### Q: Does it require jailbroken?
- **_NO, IT DOES NOT_**. The IPA is made for non-jb users. 
- **_If you are jailbroken, DO NOT use uYou+_**. All tweaks in uYou+ are available on Cydia.

***
### Q: I can't open uYouPlus after a week (AltStore/Sideloadly). It said **YouTube is no longer available**

- Apps that have been installed using a free developer account are only valid for 7 days (you can check the expire date in AltStore). For now, please re-install AltStore & uYouPlus. 
- How to Refresh apps? [AltStore](https://github.com/qnblackcat/uYouPlus/wiki/AltStore-(macOS-&-Windows)#refresh-uyouplus)/[Sideloadly](https://github.com/qnblackcat/uYouPlus/wiki/Sideloadly-(macOS-&-Windows)#refresh-uyouplus)

***
### Q: Should I remove the vanilla YouTube?
❖ You don‘t have to but you should. Keeping the vanilla YouTube app may cause issues with Google Sign-in and Cast to TV

***
### Q: I can't sign into my Google account!!!
❖ Try to delete the regular YouTube app, then re-install uYou+. If it doesn't help, try another sideload tool.

***
### Q: Why can't I see 2K/4K quality?
❖ Make sure you enable **YTUHD** in **YouTube Settings > Video quality preferences**. However, I recommend you leave YTUHD disabled.
> Attention: watching 2K/4K videos will cause many issues such as battery drain, overheating, stuttering... That's because YTUHD uses software decoder (vanilla YouTube uses hardware decoder).

***
### Q: Deep-link (aka **Open in the YouTube app**) doesn't work?
❖ It's impossible to make deep-link work. However, you can use this [Shortcut](https://shortcutsgallery.com/shortcuts/open-in-youtube/) as a workaround (tested on iOS 14). **Credit:** RandomAccessMemories#5025

***
### Q: Why does it take so long to active PiP? 
❖ Have you enabled native YouTube PiP in **YouTube Settings > General**? This is where **YouPiP** shines! 

***
### Q: The app stop playing when I turn off the screen?
❖ I‘m pretty sure you have PiP enabled. PiP will stop playing when you lock the screen. **This is iOS behavior!** Feel free to submit feedback to Apple.

***
### Q: What is **Legacy PiP**? Should I enable it?
❖ No. I wouldn't suggest you enable Legacy PiP. It is a workaround for the speed-up bug that happens on iOS 14.0 - 14.4.2. I already mentioned about **Legacy PiP** in [Known issues](#known-issues)

***
### Q: Why can't I disable Background playback?!? I turned off Background playback in uYou's settings!
- In order to enable native Picture in Picture, Background playback must be enabled by **YouPiP**. Therefore, YouTube is still running in  Background even when you disable Background playback in uYou's settings.
- If you hate Background playback that much: Extract the IPA, go to `Payload > YouTube.app > Frameworks`, delete **YouPiP.dylib**, and then re-create the IPA. Or just [build](https://github.com/qnblackcat/uYouPlus/wiki/Building) your own version of uYouPlus without YouPiP.

***
### Q: Why can't I receive push notifications?
- Push notifications will not work if you use a free developer account (limitation of sideload).
- If you have a paid developer account, take a look at [SignTools](https://github.com/SignTools/SignTools). With some effort, you can fix push notifications.

***
### Q: What is the difference between uYou normal download and uYou Local download?
❖ MiRO explained it [here](https://www.reddit.com/r/jailbreak/comments/p5jekg/update_uyou_added_uyoulocal_feature_and_much_more/)

***
### Q: Slow download speed?
❖ Well, YouTube slows down the download speed for some reasons. Let's hope MiRO92 can do something about it.

***
### Q: uYou download is not working! (Error 200: Unable to move a file from…)
- For appdb PRO users: follow [**this guide**](https://www.reddit.com/r/sideloaded/comments/pub39h/guide_how_to_fix_uyouuyou_download_not_working/) to fix uYou download not working.
- This also happens with ESign. Unfortunately, there is no fix for ESign, but you can try to use the _**Apple Developer certificate**_ instead of the _**Apple Distribution certificate**_.

***
### Q: Cast to TV not working?
❖ Remove the vanilla YouTube. 

***