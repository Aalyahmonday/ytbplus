## Method 1: theos-jailed

1. Setup [theos-jailed](https://github.com/kabiroberai/theos-jailed/wiki/Installation)

2. Ensure you have Xcode Command Line Tools installed & iOS 15 SDKs in theos/sdks

3. Clone this repo:
```
git clone --recursive https://github.com/qnblackcat/uYouPlus.git
```
4. **Important:** Open `Makefile` and edit the path to your decrypted YouTube IPA. 

5. Optional: Customize the app the way you want. I highly recommend you take a look at the [theos-jailed wiki](https://github.com/kabiroberai/theos-jailed/wiki/Usage).

6. `cd` to the project folder, run:
```
make clean package
```

7. The IPA is stored in the **packages** folder.

Note:
- I couldn‘t found a proper way to compile Alderis color picker, so we will use compiled dylib (for now).

***

## Method 2: azule

1. Setup [Azule](https://github.com/Al4ise/Azule) on your machine (macOS/Linux/iOS).

2. Download all the tweaks you want to inject. 

- [iOS Repo Updates](https://www.ios-repo-updates.com/) is a trust-able source. [cydownload](https://github.com/borishonman/cydownload) and [Windows Repo Tool](https://github.com/SarahH12099/Windows-Repo-Tool) are good alternatives.

- The sideload version of iSponsorBlock. You can get it from [my fork](https://github.com/qnblackcat/iSponsorBlock) _(thanks @Luewii for his code!)_

3. Don't forget to prepare the **decrypted** YouTube IPA. _(encrypted IPA will NOT work)_

4. Run `azule -h` in any Terminal window and follow the instruction.