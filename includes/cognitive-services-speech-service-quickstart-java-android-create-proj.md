---
author: trrwilson
ms.service: cognitive-services
ms.topic: include
ms.date: 10/15/2020
ms.author: travisw
---

1. Open Android Studio, and select **Start a new Android Studio project** in the **Welcome** window.

    ![Screenshot of the Android Studio Welcome window.](../articles/cognitive-services/Speech-Service/media/sdk/qs-java-android-01-start-new-android-studio-project.png)

1. The **Choose your project** wizard appears. Select **Phone and Tablet** and **Empty Activity** in the activity selection box. Select **Next**.

   ![Screenshot of the wizard for choosing a project.](../articles/cognitive-services/Speech-Service/media/sdk/qs-java-android-02-target-android-devices.png)

1. On the **Configure your project** page:

   1. For **Name**, enter **Quickstart**. 
   1. For **Package name**, enter **samples.speech.cognitiveservices.microsoft.com**. 
   1. For **Save location**, select a project directory. 
   1. For **Minimum API level**, select **API 23: Android 6.0 (Marshmallow)**. 
   1. Leave the two check boxes clear, and select **Finish**.

   ![Screenshot of the selections for configuring a project in the wizard.](../articles/cognitive-services/Speech-Service/media/sdk/qs-java-android-03-create-android-project.png)

Android Studio takes a moment to prepare your new Android project. Next, configure the project to know about the Azure Cognitive Services Speech SDK and to use Java 8.

[!INCLUDE [License notice](cognitive-services-speech-service-license-notice.md)]

The current version of the Cognitive Services Speech SDK is 1.21.0.

The Speech SDK for Android is packaged as an [Android Archive (AAR) file](https://developer.android.com/studio/projects/android-library), which includes the necessary libraries and required Android permissions.
It's hosted in a Maven repository at `https://azureai.azureedge.net/maven/`.

Set up your project to use the Speech SDK. Open the **Project Structure** window by selecting **File** > **Project Structure** from the Android Studio menu bar. In the **Project Structure** window, make the following changes:

1. In the list on the left side of the window, select **Project**. Edit the **Default Library Repository** settings by appending a comma and the Maven repository URL enclosed in single quotation marks: **'https:\//azureai.azureedge.net/maven/'**.

   ![Screenshot of the Project Structure window.](../articles/cognitive-services/Speech-Service/media/sdk/qs-java-android-06-add-maven-repository.png)

1. In the same window, on the left side, select **app**. Then select the **Dependencies** tab at the top of the window. Select the green plus sign (**+**), and select **Library dependency** from the drop-down menu.

   ![Screenshot of a library dependency in a project structure.](../articles/cognitive-services/Speech-Service/media/sdk/qs-java-android-07-add-module-dependency.png)

1. In the window that appears, enter the name and version of the Speech SDK for Android: **com.microsoft.cognitiveservices.speech:client-sdk:1.21.0**. Then select **OK**.
   
   The Speech SDK should now be added to the list of dependencies:

   ![Screenshot of the Speech SDK in the list of dependencies.](../articles/cognitive-services/Speech-Service/media/sdk/qs-java-android-08-dependency-added-1.0.0.png)

1. Select the **Properties** tab. For both **Source Compatibility** and **Target Compatibility**, select **1.8**.

   ![Screenshot of selections for Source Compatibility and Target Compatibility.](../articles/cognitive-services/Speech-Service/media/sdk/qs-java-android-09-dependency-added.png)

1. Select **OK** to close the **Project Structure** window and apply your changes to the project.
