# AppTransfer

Android app for exporting installed apps as APK files and sharing them to another Android phone.

Flow:

**Installed app → Download APK → .apk file → Share/Send → Other phone → Install**

### Android limitation

This first version copies the APK exposed by an app's `sourceDir`. Apps installed as Android App Bundles/split APKs, protected packages, or apps requiring additional installation components may not be transferable as one standalone APK.

### Build

Push to `main` or manually run the GitHub Actions workflow. The finished debug APK is uploaded as the `AppTransfer-debug` artifact.

The broad package-visibility permission is intended for this utility's installed-app listing and may have distribution-policy implications for app stores.
