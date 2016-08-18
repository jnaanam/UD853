# Create Project Sunshine

## 1-Setup

### Starter Code Version
To get started, do the following:

 1. Install Android Studio
 2. Learn basic [Project Structure](https://developer.android.com/studio/projects/index.html)
 3. Download [starter code](https://classroom.udacity.com/courses/ud853/lessons/1395568821/concepts/44191193530923) and import into Android Studio
 4. Run the starter code project and make sure it works. You can create a new AVD, or simply use one of the existing standard AVD profiles. *I use Nexus 6 API 23*
 5. Review the [Specific changes](https://classroom.udacity.com/courses/ud853/lessons/1395568821/concepts/44191193530923) section to understand key differences between starter code and current Android Studio templates.
 6. If you have an Android device, also [set up developer mode](https://classroom.udacity.com/courses/ud853/lessons/1395568821/concepts/15886886020923) on it right now.

At this point, you are ready to start working on course content.


### Custom Version
The Sunshine Starter project reflects the exact code thinking provided by the UD853 project when it was created more than a year ago, using **Android Studio 1.0**. The goal is simply to check off the default tasks with the working code versions given to us.

The My Sunshine App project in this same directory is an exercise in rebuilding the lesson tasks in the context of the new **Android Studio 2.1** release. The goal is to build the same app for the modern versions, using the new templates and updates tools available.

This was created with "Basic Activity" with "Use a Fragment" checked. This creates an activity with a single fragment, a Floating Action Button, and an Action Bar with a Settings menu option built-in.


## 2-Add Image Assets

Work through the [exercise to replace launcher icon] (https://classroom.udacity.com/courses/ud853/lessons/1395568821/concepts/36030988320923).

Note that in new Studio, the "Clipart" option is selected by default so switch to "Image" at which point you should be able to select the new icon from local drive.

To test: Run the app and install in emulator. The icon on launcher screen should match the image used.


## Review

Questions to review this lesson. You can view entire code at [GitHub](https://github.com/udacity/Sunshine-Version-2)

Or go [here](https://github.com/udacity/Sunshine-Version-2/blob/1.06_attach_adapter/app/src/main/java/com/example/android/sunshine/app/MainActivity.java) to see just the main application source at the end of Lesson 1.


 * What is Minimum SDK? How do you select it?
 * What is Target SDK? How is it used?
 * What are the various directories in your Android project? What are the key files you need to know?
 * What is an Activity?
 * What is a Fragment?
 * What is a Layout? What are some standard Layouts?
 * What is a View? What are standard View attributes?
 * How do you add new Image Assets (e.g., for app icon)
 * What is Gradle? How do you configure it? How do you run it?
 * What is the Android Debug Bridge (adb)? What are the common tasks you perform with adb?
 * What is a Fragment? Why should you use it?
 * What is a "User Interface" in Android?
 * What does it mean to "Inflate a Layout"?
 * What are the various Views available in the "Designer" tool? What are some popular Views?
 * Where is the "Layout" definition found in an Android project? (Hint: think 'resources')
 * What is the difference between a static Layout and a dynamic one?
 * Can any View be the "root view" of a layout file? If my "UI" has just a single View, should I still use a container "Layout" element?
 * What does "@+id" achieve in the naming of a View identifier in an XML layout file?
 * Why do we need to assign identifiers ("id") to View elements in the XML file? Is this mandatory?
 * Is the View "id" an integer or a string? Why?
 * What is Responsive Design? (what are the different orientations?)
 * Why is "AbsoluteLayout" evil? (and deprecated)
 * What are three popular Layout options? When would you use each one?
 * What are [multi-screen qualifiers](https://developer.android.com/guide/topics/resources/providing-resources.html#QualifierRules) (Hint: think small phone, large phone, small tablet, large tablet)
 * What is a Scroll View?
 * What is a [ListView](https://developer.android.com/guide/topics/ui/layout/listview.html)? (Hint: Think recycling) -- Also see [RecyclerView](https://developer.android.com/training/material/lists-cards.html) for advanced reading
 * What is an [AdapterView](https://developer.android.com/reference/android/widget/AdapterView.html)? -- Also see [Binding to Data with Adapter View](https://developer.android.com/guide/topics/ui/binding.html)
 * Can a ListView have items with different display views? (i.e., first item looks different from others, or odd items differ in appearance from even ones)
 * What is the application "Context"? How do you access it?
 * What is "R.java"? Who generates it and how is it generated?
 * What is the "android:supportsRtl" property in Android Manifest? (A: it set to true, it declares that your app supports right-to-left layouts; else only left-to-right layout supported by default)
 * What are mipmap? When do we use mipmap- folders (vs. drawable- folders)?




## Resources

 * See [Create a Project](https://developer.android.com/studio/projects/create-project.html) for workflow.
 * See [Add Code from a template](https://developer.android.com/studio/projects/templates.html) to understand what the different templates do


## Errata

### Gradle Errors

On importing Starter Code into Android Studio 1.2, you might see this message:

```
Gradle sync failed: failed to find target android-21 : /Users/nitya/Library/Android/sdk
           Consult IDE log for more details (Help | Show Log)
```
This is because Starter Code was built for the Android "Lollipop" version (older) and your current (newer) Studio install may not have all the older version SDKs.

**Solution:**
 * Go to Tools > Android > SDK Manager
 * See if Android 5.0 (API Level 21) is checked
 * Check and apply to install it if not.

 Perform any other recommended updates (e.g., build-tools, gradle) and fixes after this. On success, you should be able to run the app.

**Note:** You can also modify gradle config to require it to use the newer (installed) Android level as default. But for our current purposes we want to stick with course content first and make things work before updating to newer Android versions.

