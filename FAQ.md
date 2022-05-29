**_Hopefully, you will find the answer here!_**
***
### Q: Are you the developer of uYouPlus?
- I'm just a guy who put all the tweaks which are used in uYouPlus into a YouTube IPA. Anyone can do that if they want to (see [Building - Wiki](https://github.com/qnblackcat/uYouPlus/wiki/Building)). 
- **In short**: _I'm not the developer of uYouPlus. All the developers in [Credits](https://github.com/qnblackcat/uYouPlus#credits) are the developer of uYouPlus._

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
### Q: Should I remove the vanilla YouTube?
❖ You don‘t have to but you should. Keeping the vanilla YouTube app may cause issues with Cast to TV.

***
### Q: I can't sign into my Google account!!!
❖ If you're using a paid sigining service: contact them and ask "How to keep the original bundle ID when sideloading app". Login should work with the default bundle ID.
❖ If you're using your own paid developer account: generate a **Wildcard** profile, which allows you to use the default bundle ID of YouTube. 
❖ This problem rarely happens with free AltStore/Sideloadly users. In that case, try to remove vanilla YouTube (if existed) and re-install uYou+.

***
### Q: Why can't I see 2K/4K quality?
❖ Make sure you enable **YTUHD** in **YouTube Settings > Video quality preferences**. However, I recommend you leave YTUHD disabled.
> Attention: watching 2K/4K videos will cause many issues such as battery drain, overheating, stuttering... That's because YTUHD uses software decoder (vanilla YouTube uses hardware decoder).

***
### Q: Deep-link (aka **Open in the YouTube app**) doesn't work?
- It's impossible to fix deep-link (aka Open in the YouTube App). However, there are several workarounds:
  - [Open in YouTube Extensions](https://github.com/CokePokes/YoutubeExtensions) by @CokePokes: This is the combination of Open in YouTube shorcut & userscript below. uYouPlus included **Open in YouTube Extensions** by default, so you don't have to worry about it. However, in order to keep the extensions work correctly, you **MUST** keep the app's extensions when install the iPA (especially AltStore users). In case you're running out of add IDs (uYou+ needs 3 app IDs), you can install the shortcut/userscript separately:
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
### Q: What is the difference between uYou normal download and uYouLocal download?
❖ MiRO explained it [here](https://www.reddit.com/r/jailbreak/comments/p5jekg/update_uyou_added_uyoulocal_feature_and_much_more/)
❖ Unfortunately, uYouLocal download is not working atm. 

***
### Q: Slow download speed?
❖ Well, YouTube slows down the download speed for some reasons. Let's hope MiRO92 can do something about it.

***
### Q: uYou download is not working! (Error 200: Unable to move a file from…)
- This happens when you use an **Apple Distribution Certificate** to sign uYouPlus IPA. Please use an **Apple Developer Certificate** instead.
- For appdb PRO users: follow [**this guide**](https://www.reddit.com/r/sideloaded/comments/pub39h/guide_how_to_fix_uyouuyou_download_not_working/) to fix uYou download not working.

***
### Q: Cast to TV not working?
❖ Remove the vanilla YouTube. 

***
### Q: How many App ID does uYouPlus take? (AltStore)
- When sideloading uYouPlus via AltStore, uYouPlus will take 3 App IDs by default. One app IDs for the app itself, and two app IDs for [Open in YouTube Extensions](https://github.com/CokePokes/YoutubeExtensions/). See [here](https://github.com/qnblackcat/uYouPlus/wiki/FAQ#q-deep-link-aka-open-in-the-youtube-app-doesnt-work) for more details.
- Inshort: uYouPlus needs 3 app IDs to fully working. Remove app's extensions means no **Open in YouTube** workaround.