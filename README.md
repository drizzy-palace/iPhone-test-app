
* Extract or download an Snapchat decrypted ipa file.
* Place an symlink in the project folder named `theos` pointing to the theos-jailed folder you downloaded: `ln -s /path/to/theos-jailed/ theos`
* Run `make package`
* Run `./patchapp.sh info /path/to/your/file.ipa`
* Take the information from that and use XCode to create a Provisioning Profile
* Run `.patchapp.sh patch /path/to/Snapchat.ipa BUNDLE_ID` to inject the tweak into the .ipa (get the BUNDLE_ID from the info command)
* Install the .mobileprovision to the device
* Install the ipa to the device
