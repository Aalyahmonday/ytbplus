## Method 1: theos-jailed
### Requirement

- Xcode 13+

- theos & theos-jailed

- iOS 15 SKDs in `theos/sdks`

### Step

1. Clone this repo:
```
git clone --recursive https://github.com/qnblackcat/uYouPlus.git
```
2. **Important:** Open `Makefile` and edit the path to your decrypted YouTube IPA. 

3. Optional: Customize the app the way you want. I highly recommend you take a look at the [theos-jailed wiki](https://github.com/kabiroberai/theos-jailed/wiki/Usage).

4. `cd` to the project folder, run:
```
make clean package
```
![Screen Shot 2022-02-15 at 15 37 58](https://user-images.githubusercontent.com/52943116/154024200-f9cf8726-5536-4d68-a649-96649bc99e40.png)


5. Grab a coffee. The process might take several minutes. The IPA is stored in `./uYouPlus/packages`

***

## Method 2: azule

1. Setup [Azule](https://github.com/Al4ise/Azule) on your machine (macOS/Linux/iOS).

2. Download all the tweaks you want to inject. 

- [iOS Repo Updates](https://www.ios-repo-updates.com/) is a trust-able source. [cydownload](https://github.com/borishonman/cydownload) and [Windows Repo Tool](https://github.com/SarahH12099/Windows-Repo-Tool) are good alternatives.

- The sideload version of iSponsorBlock. You can get it from [my fork](https://github.com/qnblackcat/iSponsorBlock) _(thanks @Luewii for his code!)_

3. Don't forget to prepare the **decrypted** YouTube IPA. _(encrypted IPA will NOT work)_

4. Run `azule -h` in any Terminal window and follow the instruction.