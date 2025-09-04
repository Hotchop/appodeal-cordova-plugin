## Changes Made in plugin.xml:

### Plugin Version Updated:
- Plugin version: 3.0.5 → 3.3.0
- Package.json version: 3.0.5 → 3.3.0

### Appodeal SDK Updated:
- appodeal-2.1.11.jar → appodeal-3.3.0.jar
- appodeal-banner-view-2.3.0.jar → appodeal-banner-view-3.3.0.jar

### Network Adapter SDKs Updated:
- AppLovin: 7.5.0 → 12.6.0
- Chartboost: 6.6.3 → 9.7.0
- InMobi: 6.2.3 → 10.7.4
- Ogury: 2.1.15 → 5.6.0
- Picasso: 2.5.2 → 2.8.0
- Unity Ads: 2.1.0 → 4.12.2
- Yandex Metrica: 2.73 → 6.4.0
- StartApp: 3.6.7 → 4.11.5

## IMPORTANT: Manual Steps Required

⚠️ **The JAR files referenced in plugin.xml have been updated to newer versions, but the actual JAR files need to be replaced manually.**

### To Complete This Update:

1. **Download Latest Appodeal SDK**:
   - Visit: https://www.appodeal.com/sdk/documentation?framework=1&full=1&platform=1
   - Download the latest Android SDK (3.3.0 or newer)
   - Extract the SDK files

2. **Replace JAR Files**:
   - Replace `libs/Android/appodeal-2.1.11.jar` with `appodeal-3.3.0.jar`
   - Replace `libs/Android/appodeal-banner-view-2.3.0.jar` with `appodeal-banner-view-3.3.0.jar`
   - Update all network adapter JAR files with the versions specified above

3. **Update iOS SDK** (if needed):
   - Download latest iOS SDK from Appodeal
   - Replace the Appodeal.framework and related files in `libs/iOS/`

4. **Update AndroidManifest.xml entries** (if needed):
   - Check if new SDK version requires additional manifest entries
   - Update activity declarations if changed in new SDK

5. **Test the Plugin**:
   - Build a test project with the updated plugin
   - Verify all ad formats work correctly
   - Test on both Android and iOS

## Notes:
- SDK versions chosen are modern stable versions as of 2024-2025
- Some network adapters may require additional configuration changes
- Always test thoroughly before deploying to production
- Check Appodeal's changelog for any breaking changes

## References:
- Appodeal Android SDK: https://www.appodeal.com/sdk/documentation?framework=1&platform=1
- Appodeal iOS SDK: https://www.appodeal.com/sdk/documentation?framework=20&platform=4
