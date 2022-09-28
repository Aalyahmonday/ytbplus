**_Hopefully, you will find the answer here!_**
***
### Q: "Google couldn't confirm this attempt to sign in is safe. If you think this is a mistake, you can close and try again to sign in." warning when signing in.
- **The issue has been solved in [v17.37.3-2.1](https://github.com/qnblackcat/uYouPlus/releases/tag/v17.37.3-2.1) or higher. However, Google can easily break it again if they want. Therefore don't be surprised if it suddenly stop working.**
- For more details about the problem, check out [this disscussion](https://github.com/qnblackcat/uYouPlus/discussions/447).

***
### Q: "You can't sign in to this app because Google can't confirm that it's safe" warning when signing in.
#### ☞ **Update**: this issue has been addressed on [v17.33.2-2.1](https://github.com/qnblackcat/uYouPlus/releases/tag/v17.33.2-2.1) and higher. You don‘t need to follow the trick below anymore. Just make sure you‘re on the newest version!

<details>
  <summary>Expand</summary>

#### ☞ The situation:
Google has added a new implementation that prevents users from signing in to modified YouTube apps (see [Less secure apps](https://support.google.com/accounts/answer/6010255?hl=en)). Basically, If the bundle ID of the app is modified, Google won't let us sign in. But **if you're already signed it, you will be fine**. Just don't remove the app, so you don't need to sign in again.

#### ☞ Which choice do we have now? (
Fortunately, there are two workarounds (not guarantee working 100%):
- **Method 1**: Keeping the original bundle ID of YouTube (`com.google.ios.youtube`) when sideloading YouTube: This is definitely not a real solution because it isn't available for free users. You’ll need a paid developer certificate & a wildcard provisioning profile to achieve it.
- **Method 2**: This might be a bit complicated, but everyone can follow it _(discovered by @Cao Đức Phát)_:
1. First, try to login to YouTube like normal, you’ll see the “You can't sign in to this app…” warning.
2. Hold and copy the URL like [this](https://camo.githubusercontent.com/be528e9123cba5a5348ddbf2912b70397c8a1e742d54df0a7a8d14bdfe152bfe/68747470733a2f2f6d656469612e646973636f72646170702e6e65742f6174746163686d656e74732f3835383635373535333738313232373537302f313030353035313538303530363139343030312f494d475f32303232303830355f3136353630312e6a7067). 
3. Open the URL in a new Safari private (incognito) window, you should be able to sign in to Google now.
4. After signing in to Google, you will be asked to “Open in YouTube” > Done!

=> For those who still having trouble following the second method, I made a video [here](https://drive.google.com/file/d/17c9I419tdBf91oTeL0MQGNm4KlrVmlMk/view?usp=drivesdk).

**PS: again, these workarounds are old and no longer needed. All you need to do is update to the latest version of uYouPlus.**
</details>

***
### Q: App crashes on iOS 16?
- ~~uYou doesn't work on iOS 16 , so don’t bother trying.~~ 
- uYouPlus [v17.24.4-2.1](https://github.com/qnblackcat/uYouPlus/releases/tag/v17.24.4-2.1) and higher supports iOS 16!

***
### Q: Are you the developer of uYouPlus?
- I'm just a guy who put all the tweaks which are used in uYouPlus into a YouTube IPA. Anyone can do that if they want to (see [Building - Wiki](https://github.com/qnblackcat/uYouPlus/wiki/Building)). 
- **In short**: _I'm not the developer of uYouPlus. All the developers who are mentioned in [Credits](https://github.com/qnblackcat/uYouPlus#credits) are the developer of uYouPlus._

***
### Q: I want to add my language to uYouPlus. How do I do that?
- Translator are always welcome. If your language already exists then feel free to check it and/or improve it:
  1. Fork uYouPlus repo
  2. Go to `lang > uYouPlus.bundle`. Duplicate the template.lproj folder, and edit the duplicated folder's name to your <lang_code>.lproj id.
For example: <ru.lproj> for Russia. For more details, visit: https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes
  3. Translate each line below after each =
  4. Open a Pull Request

- You can also add your localization to [YouPiP](https://github.com/PoomSmart/YouPiP/tree/main/layout/Library/Application%20Support/YouPiP.bundle), [YTUHD](https://github.com/PoomSmart/YTUHD/tree/master/layout/Library/Application%20Support/YTUHD.bundle) and [Return YouTube Dislike](https://github.com/PoomSmart/Return-YouTube-Dislikes/tree/main/layout/Library/Application%20Support/RYD.bundle). The process is the same.

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
- If you are jailbroken but still want to use uYouPlus, you must sideload it with AltStore, Sideloadly, Reprovision... Using AppSync Unifield & Filza will not work (app crashes on launching).

***
### Q: Does it support ARM mac?
- **_NO, IT DOES NOT_**. 
- I also don’t own an ARM mac, please don’t ask me to add support for ARM mac. Perhaps other developers could do that.

***
### Q: How do I refresh uYouPlus?
- AltStore users: see [here](https://github.com/qnblackcat/uYouPlus/wiki/AltStore-(macOS-&-Windows-&-Linux)#refresh-uyouplus).
- Sideloadly users: see [here](https://github.com/qnblackcat/uYouPlus/wiki/Sideloadly-(macOS-&-Windows)#refresh-uyouplus).

***
### Q: I can't open uYouPlus after a week (AltStore/Sideloadly). It said **YouTube is no longer available**. 
- Apps that have been installed using a free developer account are only valid for 7 days (you can check the expiry date in AltStore). Please re-install AltStore & uYouPlus.
- How to Refresh apps? See the answer above.

***
### Q: YouTube crashes when opening uYou's settings?
- This has been addressed in [v17.34.3-2.1](https://github.com/qnblackcat/uYouPlus/releases/tag/v17.34.3-2.1) or higher.

***
### Q: Error `Failed to load Info.plist from bundle at path /private/var/container/Bundle/Application...`
- See this: 
https://github.com/qnblackcat/uYouPlus/issues/360#issuecomment-1214204795

***
### Q: Should I remove the vanilla YouTube? Cast to TV not working?
❖ You don‘t have to but you should. However, keeping the vanilla YouTube app may cause issues with Cast to TV. Remove the stock YouTube app in that case.

***
### Q: I see ads when casting to TV?
- Let's make it simple: Cast to TV means you tell your TV play a video. But your TV loads that video directly from YouTube, not from your phone. 
- If you use AirPlay then you won't see any ads, because you're streaming your video directly to your TV. 

***
### Q: I signed in, but got "Error fetching channel list for account Tap to try again" error!
- This should be fixed in [v17.21.3-2.1](https://github.com/qnblackcat/uYouPlus/releases/tag/v17.21.3-2.1) and newer. If not, see below:
  - If you're using a paid sigining service: contact your signing service and ask them "How to keep the original bundle ID when sideloading app". Login should work with the default bundle ID.
  - If you're using your own paid developer account: generate a **wildcard** profile, which allows you to use the default bundle ID of YouTube. 
  - AltStore/Sideloadly users: make sure the bundle ID of the IPA was not modified. It should be `com.google.ios.youtube`

***
### Q: The timestamp of videos in History, Playlist, Watch later is missing!
- Please read the changelog closely:
> Workaround for missing the video's timestamp in Watch History/Playlist: Go to uYou's settings > Other Settings and [Disable](https://user-images.githubusercontent.com/52943116/150642296-5de53fc7-a1ea-4b3d-96f4-25c9ca8b8f81.JPG) "Remove YouTube Ads"

***
### Q: My watch history not syncing?
- Check your DNS setting. Every time people complain about this issue, it is due to DNS configuration.

***
### Q: Age restricted (offensive/inappropriate) videos not playing?
- Go to uYou's setting > Turn off **Disable Age Restriction**.

***
### Q: Why can't I see 2K/4K quality?
- Make sure you enable **YTUHD** in **YouTube Settings > Video quality preferences**. However, I recommend you leave YTUHD disabled unless you use TrollStore to install uYouPlus.
- Watching 2K/4K videos may cause several issues, such as battery drain, overheating, stuttering... That's because YTUHD uses software decoder (vanilla YouTube uses hardware decoder). PoomSmart explained it [here](https://github.com/PoomSmart/YTUHD#sideloading). **However, YTUHD works perfectly fine when the app was installed by TrollStore.**

***
### Q: Deep-link (aka **Open in the YouTube app**) doesn't work?
- If uYouPlus was installed via TrollStore, then Deep link should work out of the box.
- If you can't use TrollStore, then it is impossible to fix deep link. However, there are several workarounds:
  - [Open in YouTube Extensions](https://github.com/CokePokes/YoutubeExtensions) by @CokePokes: This is the combination of Open in YouTube shorcut & userscript below. **uYouPlus included Open in YouTube Extensions by default**, so you don't have to worry about it. However, in order to keep the extensions work correctly, you **MUST** keep the app's extensions when install the iPA (especially AltStore users). In case you're running out of add IDs (uYou+ needs 3 app IDs), you can install the shortcut/userscript separately:
    - Safari extension & Userscript: iOS 15 users can follow [this workaround](https://github.com/qnblackcat/uYouPlus/issues/69).
    - iOS 14 users can use [Open in YouTube](https://shortcutsgallery.com/shortcuts/open-in-youtube/) shortcut.
  - [Opener](https://apps.apple.com/us/app/opener-open-links-in-apps/id989565871) is a paid app from AppStore that allows you to open links from the web in apps.

***
### Q: Why does it take so long to active PiP? 
❖ Have you enabled native YouTube PiP in **YouTube Settings > YouPiP**? This is where **YouPiP** shines! 

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
- Pusn notifications work out of the box if the app was installed by TrollStore.
- Push notifications will not work on free developer account (limitation of sideload).
- If you have a paid developer account, take a look at [SignTools](https://github.com/SignTools/SignTools). With some effort, you can fix push notifications.
- Bear in mind that not all signing services support Push notifications.

***
### Q: What is the difference between uYou normal download and uYouLocal download?
- MiRO explained it [here](https://www.reddit.com/r/jailbreak/comments/p5jekg/update_uyou_added_uyoulocal_feature_and_much_more/)
- From my experience, uYouLocal has a better download speed!?

***
### Q: Slow download speed?
❖ Well, YouTube slows down the download speed. Let's hope MiRO92 could do something about it.

***
### Q: uYou download is not working! (Error 200: Unable to move a file from…)
- ~~This happens when you use an **Apple Distribution Certificate** to sign uYouPlus IPA. Please use an **Apple Developer Certificate** instead.~~
- ~~For appdb PRO users: follow [**this guide**](https://www.reddit.com/r/sideloaded/comments/pub39h/guide_how_to_fix_uyouuyou_download_not_working/) to fix uYou download not working.~~
- Looks like the fix is not working [anymore](https://github.com/qnblackcat/uYouPlus/issues/238). Waiting for the new update of uYou is our only hope.
- This issue should not happen when you use Trollstore.

***
### Q: How many App ID does uYouPlus take? (AltStore)
- When sideloading uYouPlus via AltStore, uYouPlus will take 3 App IDs by default. One app IDs for the app itself, and two app IDs for [Open in YouTube Extensions](https://github.com/CokePokes/YoutubeExtensions/). See [here](https://github.com/qnblackcat/uYouPlus/wiki/FAQ#q-deep-link-aka-open-in-the-youtube-app-doesnt-work) for more details.
- Inshort: uYouPlus needs 3 app IDs to fully working. Remove app's extensions means no **Open in YouTube** workaround.