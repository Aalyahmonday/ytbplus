# Method 1: Github action
## Requirement:
- A Github account.
- A decrypted YouTube ipa. You must upload it to a cloud storage service (Dropbox, OneDrive, Google Drive or whatever you want). After that, get the direct download link to the IPA.

## Step:
1. Fork this repository.
2. Upload the decrypted YouTube IPA to a cloud storage that can provide direct link to the IPA. For example: DropBox, OneDrive...
3. In your forked repository, go to the **Actions** tab > Select **Build and Release uYouPlus** action > **Run workflow** > Enter the direct link to the decrypted YouTube IPA.

![Screenshot 2024-02-27 at 21 57 52](https://github.com/qnblackcat/uYouPlus/assets/52943116/1688dd42-4ff0-44a5-b1f0-c21476246312)

4. That's it! Grab a coffee ☕️ It will take a while. You will see the IPA in the **Releases tab** of your repository.

***

# Method 2: theos-jailed
## Requirement:
- Xcode 14+ & Xcode Command Line Tools
- theos & theos-jailed
- A patched iOS 16.5 SDK (with Private Frameworks) in `theos/sdks`: https://github.com/theos/sdks

## Step:
1. Clone this repo: `git clone --recursive https://github.com/qnblackcat/uYouPlus.git`
2. Update submodules: `cd ./uYouPlus && git submodule update --remote --merge`
3. Make the `build.sh` script executable: `chmod +x ./build.sh`
4. _Optional: open `Makefile` and add or remove any tweaks you want. You can also edit the bundle ID / display name of the app. I highly recommend you take a look at the theos-jailed [wiki](https://github.com/kabiroberai/theos-jailed/wiki/Usage)._
5. Run the buildapp script: `./build.sh`, provide the decrypted YouTube IPA when asked.

```
$ git clone --recursive https://github.com/qnblackcat/uYouPlus.git
$ cd ./uYouPlus && git submodule update --remote --merge
$ chmod +x ./build.sh
$ ./build.sh
```
![Screen Shot 2](https://user-images.githubusercontent.com/52943116/168122339-cfa388cb-4956-48cc-a4d5-cfba22612bbf.png)

✔︎ That's it! Grab a coffee ☕️ It will take a while. The IPA is stored in `./uYouPlus/packages`