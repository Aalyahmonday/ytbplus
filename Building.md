## _It seems like you want to make your own version of YouTube..._

## Method 1: azule

1. Setup [Azule](https://github.com/Al4ise/Azule) on your machine (macOS/Linux/iOS).

2. Download all the tweaks you want to inject. 

- [iOS Repo Updates](https://www.ios-repo-updates.com/) is a trust-able source. [cydownload](https://github.com/borishonman/cydownload) and [Windows Repo Tool](https://github.com/SarahH12099/Windows-Repo-Tool) are good alternative.

- The sideloaded version of iSponsorBlock is here ([Luewii's fork](https://github.com/Luewii/iSponsorBlock)).

3. Don't forget to prepare the **decrypted** YouTube IPA.

4. Run `azule` in any Terminal window and follow the instruction.

5. Select `1. Inject tweaks`, then Drag & drop the **decrypted** YouTube IPA as long as your tweaks into the azule window. Other azule options are optional.

6. Done! Azule will take care of the rest!

***

## Method 2: theos-jailed

1. Setup [theos-jailed](https://github.com/kabiroberai/theos-jailed/wiki/Installation)

2. Clone this repo:
```
git clone https://github.com/qnblackcat/uYouPlus.git
```
3. **Important:** Open `Makefile` and edit the path to your decrypted YouTube IPA. 

4. Optional: Modify the app & the tweak the way you want. I highly recommend you take a look at the [theos-jailed wiki](https://github.com/kabiroberai/theos-jailed/wiki/Usage).

5. `cd` to the project folder, run:
```
make clean package
```

