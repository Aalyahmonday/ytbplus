# Method 1: Github action
## Requirement:
- A Github account.
- A decrypted YouTube ipa. You must upload it to your cloud storage service (Dropbox, OneDrive, GG Drive... or whatever you want). After that, get the direct download link to the IPA.

## Step:
1. Fork this repository.
2. In your forked repository, go to the **Actions** tab > Select **Build and Release uYouPlus** action > **Run workflow** > Enter everything it requires. _Make sure you use a direct link to the IPA._

![Screen Shot 2](https://user-images.githubusercontent.com/52943116/175647144-c49ea7b5-d74a-4450-9819-2f7b5b462d0a.png)

3. That's it! Grab a coffee ☕️ The process might take several minutes. You will see the IPA in the **Releases tab** of your repository.

***

# Method 2: theos-jailed
## Requirement:
- Xcode 13+ & Xcode Command Line Tools
- theos & theos-jailed
- iOS 15 SDK in `theos/sdks`

## Step:
1. Clone this repo: `git clone --recursive https://github.com/qnblackcat/uYouPlus.git`
2. Update submodules: `cd ./uYouPlus && git submodule update --remote --merge`
3. Make the `buildapp.sh` script executable: `chmod +x ./buildapp.sh`
4. _Optional: add or remove any tweaks you want. I highly recommend you take a look at the theos-jailed [wiki](https://github.com/kabiroberai/theos-jailed/wiki/Usage)._
5. Run the buildapp script: `./buildapp.sh`, and drag & drop the decrypted YouTube IPA into the terminal window when it asks you:

```
git clone --recursive https://github.com/qnblackcat/uYouPlus.git
cd ./uYouPlus && git submodule update --remote --merge
chmod +x ./buildapp.sh
./buildapp.sh
```
![Screen Shot 2](https://user-images.githubusercontent.com/52943116/168122339-cfa388cb-4956-48cc-a4d5-cfba22612bbf.png)

✔︎ That's it! Grab a coffee ☕️ The process might take several minutes. The IPA is stored in `./uYouPlus/packages`