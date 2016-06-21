# Create Project Sunshine

To get started, do the following:

 1. Install Android Studio
 2. Learn basic [Project Structure](https://developer.android.com/studio/projects/index.html)
 3. Download [starter code](https://classroom.udacity.com/courses/ud853/lessons/1395568821/concepts/44191193530923) and import into Android Studio
 4. Run the starter code project and make sure it works.
 5. Review the [Specific changes](https://classroom.udacity.com/courses/ud853/lessons/1395568821/concepts/44191193530923) section to understand key differences between starter code and current Android Studio templates.

At this point, you are ready to start working on course content.

## Errata

1. On importing Starter Code into Android Studio 1.2, you might see this message:

```
Gradle sync failed: failed to find target android-21 : /Users/nitya/Library/Android/sdk
           Consult IDE log for more details (Help | Show Log)
```
This because Starter Code was built for the Android "Lollipop" version (older) and your current (newer) Studio install may not have all the older version SDKs.

Solution:
 * Go to Tools > Android > SDK Manager
 * See if Android 5.0 (API Level 21) is checked
 * Check and apply to install it if not.
 * Perform any other recommended updates (e.g., build-tools, gradle) and fixes.

 On success, you should be able to run the app.

Note: You can also modify gradle config to require it to use the newer (installed) Android level as default. But for our current purposes we want to stick with course content first and make things work before updating to newer Android versions.