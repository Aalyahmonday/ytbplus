**_Hopefully, you will find the answer here!_**
***
### Q: App crashes on iOS 16?
- ~~uYou doesn't work on iOS 16 , so don’t bother trying.~~ 
- uYouPlus [v17.24.4-2.1](https://github.com/qnblackcat/uYouPlus/releases/tag/v17.24.4-2.1) and higher supports iOS 16!

***
### Q: Are you the developer of uYouPlus?
- I'm just a guy who put all the tweaks which are used in uYouPlus into a YouTube IPA. Anyone can do that if they want to (see [Building - Wiki](https://github.com/qnblackcat/uYouPlus/wiki/Building)). 
- **In short**: _I'm not the developer of uYouPlus. All the developers who are mentioned in [Credits](https://github.com/qnblackcat/uYouPlus#credits) are the developer of uYouPlus._

***
### Q: Is uYouPlus safe?
- Eww, I'm afraid that I cannot answer this question. While most of the tweaks that are used in uYouPlus are open-source, there are two things that are not open-source:
  - **uYou**: uYou is not open-source. But MiRO92 - the developer of uYou, is a very well-known and talent developer in jailbreak community. If you don't trust him, then I think you have no one left to trust 🤷‍♂️
  - The YouTube ipa: you always can decrypt YouTube yourself. 
- After all, I highly recommend you build your own iPA of uYouPlus. See [Building - Wiki](https://github.com/qnblackcat/uYouPlus/wiki/Building)

***
### Q: I got the IPA. How do I install uYouPlus?
❖ There are many tools to sideload IPA to your phone. AltStore and Sideloadly are recommended. See [Installation - Wiki](https://github.com/qnblackcat/uYouPlus/wiki/Installation) for more info. 

***
### Q: Does it require jailbroken?
- **_NO, IT DOES NOT_**. The IPA is made for non-jb users. 
- **_If you are jailbroken, DO NOT use uYou+_**. All tweaks in uYou+ are available on Cydia.

***
### Q: How do I refresh uYouPlus?
- AltStore users: please see [here](https://github.com/qnblackcat/uYouPlus/wiki/AltStore-(macOS-&-Windows-&-Linux)#refresh-uyouplus).
- Sideloadly users: please see [here](https://github.com/qnblackcat/uYouPlus/wiki/Sideloadly-(macOS-&-Windows)#refresh-uyouplus).

***
### Q: I can't open uYouPlus after a week (AltStore/Sideloadly). It said **YouTube is no longer available**. 
- Apps that have been installed using a free developer account are only valid for 7 days (you can check the expiry date in AltStore). For now, please re-install AltStore & uYouPlus.
- How to Refresh apps? See the answer above.

***
### Q: YouTube crashes when opening uYou's settings?
- Use v16.42.3 if the app crashes when opening uYou's setting ([Issue #10](https://github.com/qnblackcat/uYouPlus/issues/10)). Otherwise, I would not recommend you using v16.42.3. [FAQ - Building](https://github.com/qnblackcat/uYouPlus/wiki/building) will tell you how to build your own version of uYouPlus.
- Apparently, this issue usually only happens on early versions of iOS 15.

***
### Q: Error `Failed to load Info.plist from bundle at path /private/var/container/Bundle/Application...`
- I assume you're using AltStore or Sideloadly. In either case:
  - Fully uninstall AltStore & uYouPlus.
  - Reinstall AltStore & latest version of uYouPlus.
- You only need to do this once. The issue should not happen anymore.

***
### Q: Should I remove the vanilla YouTube? 
❖ You don‘t have to but you should. However, keeping the vanilla YouTube app may cause issues with Cast to TV.

***
### Q: Cast to TV not working?
❖ Remove the vanilla YouTube.

***
### Q: I see ads when casting to TV?
- Let's make it simple: Cast to TV means you tell your TV play a video. But your TV loads that video directly from YouTube, not from your phone. 
- If you use AirPlay then you won't see any ads, because you're streaming your video directly to your TV. 

***
### Q: I can't sign into my Google account!!! 
- This should be fixed in [v17.21.3-2.1](https://github.com/qnblackcat/uYouPlus/releases/tag/v17.21.3-2.1) and newer. If not, see below:
  - If you're using a paid sigining service: contact your signing service and ask them "How to keep the original bundle ID when sideloading app". Login should work with the default bundle ID.
  - If you're using your own paid developer account: generate a **wildcard** profile, which allows you to use the default bundle ID of YouTube. 
  - This problem rarely happens with free AltStore/Sideloadly users. In that case, try to remove vanilla YouTube (if existed) and re-install uYou+.

***
### Q: The timestamp of videos in History, Playlist, Watch later is missing!
- Please read the changelog closely:
> Workaround for missing the video's timestamp in Watch History/Playlist: Go to uYou's settings > Other Settings and [Disable](https://user-images.githubusercontent.com/52943116/150642296-5de53fc7-a1ea-4b3d-96f4-25c9ca8b8f81.JPG) "Remove YouTube Ads"

***
### Q: Why can't I see 2K/4K quality?
- Make sure you enable **YTUHD** in **YouTube Settings > Video quality preferences**. However, I recommend you leave YTUHD disabled.
- **Attention**: watching 2K/4K videos may cause several issues, such as battery drain, overheating, stuttering... That's because YTUHD uses software decoder (vanilla YouTube uses hardware decoder). PoomSmart explained it [here](https://github.com/PoomSmart/YTUHD#sideloading).

***
### Q: Deep-link (aka **Open in the YouTube app**) doesn't work?
It's impossible to fix deep-link (aka Open in the YouTube App). However, there are several workarounds:
- [Open in YouTube Extensions](https://github.com/CokePokes/YoutubeExtensions) by @CokePokes: This is the combination of Open in YouTube shorcut & userscript below. **uYouPlus included Open in YouTube Extensions by default**, so you don't have to worry about it. However, in order to keep the extensions work correctly, you **MUST** keep the app's extensions when install the iPA (especially AltStore users). In case you're running out of add IDs (uYou+ needs 3 app IDs), you can install the shortcut/userscript separately:
  - Safari extension & Userscript: iOS 15 users can follow [this workaround](https://github.com/qnblackcat/uYouPlus/issues/69).
  - iOS 14 users can use [Open in YouTube](https://shortcutsgallery.com/shortcuts/open-in-youtube/) shortcut.
- [Opener](https://apps.apple.com/us/app/opener-open-links-in-apps/id989565871) is a paid app from AppStore that allows you to open links from the web in apps.

***
### Q: Why does it take so long to active PiP? 
❖ Have you enabled native YouTube PiP in **YouTube Settings > General**? This is where **YouPiP** shines! 

***
### Q: The app stop playing when I turn off the screen?
❖ I‘m pretty sure you have PiP enabled. PiP will stop playing when you lock the screen. **This is iOS behavior!** Feel free to send a feedback to Apple.

***
### Q: What is **Legacy PiP**? Should I enable it?
- No. I wouldn't suggest you enable Legacy PiP unless you tired of the [speed-up bug](https://github.com/PoomSmart/YouPiP/issues/29).
- Turn on Legacy PiP also breaks the Default video quality feature of uYou and/or YouTube.

***
### Q: Why can't I disable Background playback?!? I turned off Background playback in uYou's settings!
- In order to enable native Picture in Picture, Background playback must be enabled by **YouPiP**. Therefore, YouTube is still running in  Background even when you disable Background playback in uYou's settings.
- If you hate Background playback that much: Extract the IPA, go to `Payload > YouTube.app > Frameworks`, delete **YouPiP.dylib**, and then re-create the IPA. Or just [build](https://github.com/qnblackcat/uYouPlus/wiki/Building) your own version of uYouPlus without YouPiP.

***
### Q: Why can't I receive push notifications?
- Push notifications will not work if you use a free developer account (limitation of sideload).
- If you have a paid developer account, take a look at [SignTools](https://github.com/SignTools/SignTools). With some effort, you can fix push notifications.
- Bear in mind that not all signing services support Push notifications.

***
### Q: What is the difference between uYou normal download and uYouLocal download?
- MiRO explained it [here](https://www.reddit.com/r/jailbreak/comments/p5jekg/update_uyou_added_uyoulocal_feature_and_much_more/)

***
### Q: Slow download speed?
❖ Well, YouTube slows down the download speed. Let's hope MiRO92 can do something about it.

***
### Q: uYou download is not working! (Error 200: Unable to move a file from…)
- ~~This happens when you use an **Apple Distribution Certificate** to sign uYouPlus IPA. Please use an **Apple Developer Certificate** instead.~~
- ~~For appdb PRO users: follow [**this guide**](https://www.reddit.com/r/sideloaded/comments/pub39h/guide_how_to_fix_uyouuyou_download_not_working/) to fix uYou download not working.~~
- Looks like the fix is not working [anymore](https://github.com/qnblackcat/uYouPlus/issues/238). Waiting for the new update of uYou is our only hope.

***
### Q: How many App ID does uYouPlus take? (AltStore)
- When sideloading uYouPlus via AltStore, uYouPlus will take 3 App IDs by default. One app IDs for the app itself, and two app IDs for [Open in YouTube Extensions](https://github.com/CokePokes/YoutubeExtensions/). See [here](https://github.com/qnblackcat/uYouPlus/wiki/FAQ#q-deep-link-aka-open-in-the-youtube-app-doesnt-work) for more details.
- Inshort: uYouPlus needs 3 app IDs to fully working. Remove app's extensions means no **Open in YouTube** workaround.