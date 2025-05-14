Zync Flutter - Docs        

documentation for

* * *

Main

*   [Introduction](#introduction)
*   [System required](#system_requried)

* * *

Project changes*   [Change Base URL](#change_base_url)
*   [Change package name](#change_package_name)
*   [Change app name](#change_app_name)
*   [Change app color](#change_app_color)
*   [Change app font family](#change_app_font_family)
*   [Change app icon](#change_app_icon)

* * *

Firebase*   [Adding firebase to app](#adding_firebase_to_app)
*   [Add Android app](#android_app_add_in_Firebase)
*   [Add iOS app](#ios_app_add_in_Firebase)
*   [Email sign in](#email_sign_in)
*   [Enable firestore](#enable_firestore)

* * *

Agora*   [Setup agora](#setup_agora)

* * *

Branch.io*   [Branch.io setup](#branch_io_setup)

* * *

*   [Revenuecat](#revenuecat)
*   [Google Admob](#google_admob)
*   [Create application build](#create_build)
*   [Update info](#update_info)

Zync
====

The Ultimate Flutter Social Media

Introduction
============

Zync app is an ultimate social media script built with flutter and Laravel as backend. It offers many advanced features and functions like Feed (Images, Videos, Text), Stories, Chat, Chat Rooms, Manage Chat Rooms & Members, Random Profiles, Interests, Push Notifications And Lot more... This package contains fully functional Zync flutter app, Backend, Database file & documentation. Using this script, any individual or company can save 100s of hours and publish twitter like social media app within couple of hours.

System Required
===============

*   **Gmail** Account credentials for Firebase
    
*   **Apple** developer account credentials : [Create Account]( https://developer.apple.com/account)
    
*   **Android Studio** : [Download](https://developer.android.com/studio?gclid=CjwKCAjw04yjBhApEiwAJcvNodX3HCvOUdJv3NZQAI0ppZd7NoKWmhErYmITzfJZePTg5qNZHBQRzBoC2JoQAvD_BwE&gclsrc=aw.ds)
    
*   **Flutter Sdk** : [Download](https://docs.flutter.dev/get-started/install)
    
*   **Agora** Account : [Create Account](https://console.agora.io/)
    
*   **Branch.io** Account : [Create Account](https://dashboard.branch.io)
    
*   **Xcode** (Only Mac Users).
    
*   **RevenueCat** Account : [Create Account](https://www.revenuecat.com/)
    

Change Base URL
===============

*   Find the **Zync\_backend.zip** from the folder downloaded from codecanyon and open in android studio.
    
*   Open **Zync>lib/utils/const.dart**
    
*   Replace **"baseURL"** with your **Admin Panel URL** (https://yourdomain.com/)
    
*   Note : Make sure you have added "/" at the last.
    

Change package name
===================

*   **Android**
    

*   Step 1 : Go to **android > app**
    
*   Step 2 : Click to **build.gradle**
    
*   Step 3 : Here, change the only **applicationId** And it's done.
    

![android](https://docs.retrytech.com/asset/img/doctor/android_package_name.png)

*   **iOS**
    

*   **Step 1 :** Now right click on **iOS** directory, **flutter > Open iOS module in Xcode**
    

![iOS_package_name_1](https://docs.retrytech.com/asset/img/doctor/iOS_package_name_1.png)

Once the project gets opened in Xcode successfully, follow the steps below.

*   Step 2 : Go to **runner > Signing & Capabilities**
    
*   Step 3 : Change your **bundle identifier** as you want, and it's done.
    

![iOS_package_name_2](https://docs.retrytech.com/asset/img/doctor/iOS_package_name_2.png)

Change app name
===============

*   **Android**
    

*   **Step 1 :** Go to **android > app > src > main > AndroidManifest.xml** and make changes shown in the below image.
    

![android_app_name](https://docs.retrytech.com/asset/img/doctor/android_app_name.png)

*   **iOS**
    

*   **Step 1 :** Now right click on iOS directory **flutter > Open iOS module in Xcode**
    

![iOS_package_name_1](https://docs.retrytech.com/asset/img/doctor/iOS_package_name_1.png)

*   **Step 2 :** Now go to **Runner > General > Display Name**, change it as you want.
    

![iOS_app_name](https://docs.retrytech.com/asset/img/doctor/iOS_app_name.png)

Change app color
================

*   **Step 1 :** Now go to your project **lib > utilities > const.dart** as shown in the below image.
    

![change_app_color](https://docs.retrytech.com/asset/img/change_app_color_1.png)

Change app font family
======================

*   **Step 1 :** Select any font from google font
    

Here’s how you download the font:

*   Visit the [https://fonts.google.com/](https://fonts.google.com/)
    
*   Search for your font.
    
*   Once you find it, click to open.
    
*   Click on the Download Family button on the top right side of your screen.
    
*   Extract the compressed file.
    

![payment_1](https://docs.retrytech.com/asset/img/font_1.png)

*   **Step 2 :** Import the Font into Project
    

To import the Font in your project:

*   Copy-Paste **\[font\].ttf** file into the fonts folder.
    

![payment_1](https://docs.retrytech.com/asset/img/font_2.png)

*   **Step 3 :** Add Font to Pubspec.yaml
    

To add Font to pubspec.yaml file:

*   Replace the family name with your font family. To get the family name, simply take the first part before the dash sign (-). For example, if the downloaded font name is **Montserrat-Regular** , take the **Montserrat** as your family name
    
*   Go to **pubspec.yaml** file:
    
*   Replace the **asset** path with the path where your font is residing.
    
*   Then **pub get** to successfully load your font
    

![payment_1](https://docs.retrytech.com/asset/img/font_3.png)

Change app icon
===============

*   **Step 1 :** Generating Different Sized Icons
    

Go to [https://www.appicon.co/](https://www.appicon.co/) and **upload** the icon image and tick the **iPhone** and **Android** options and **click on Generate.** This site generates different sized Icons for both android and IOS at the same time.

![payment_1](https://docs.retrytech.com/asset/img/change_icon_1.png)

It will Download the Zip file named AppIcons with the android and Assets.xcassets named folders along with images for appstore and playstore which can be directly uploaded as an icon in both the stores

![payment_1](https://docs.retrytech.com/asset/img/change_icon_2.png)

Now, open your Project in Android Studio.

*   **Step 2 :** Adding Icons in Android.
    

Navigate to **android/app/src/main/res** and right-click on res folder and click "open in Finder". Now delete all the mipmap folders in res folder and paste the mipmap folders from AppIcon/android folder which you have downloaded.

![payment_1](https://docs.retrytech.com/asset/img/change_icon_4.png)

*   **Step 3 :** Adding Icons in IOS
    

Now navigate to the **ios/Runner/Assets.xcassets.** Now after you are in Runner folder, right-click on Runner folder and click “open in Finder”. Now delete the Assets.xcassets folder and paste the Assets.xcassets folder from AppIcon/Assets.xcassets which you have downloaded.

![payment_1](https://docs.retrytech.com/asset/img/change_icon_3.png)

*   **Step 4 :** Run the Application
    

After manually changing the images in android and IOS folders now go to lib/main.dart and run the flutter project using the below command in the flutter console.

`flutter run`

![payment_1](https://docs.retrytech.com/asset/img/change_icon_5.png)

Configure Firebase
==================

*   Go to the firebase project you might created while following backend documentation.
    
*   If you don't have, follow the steps below and create one project.
    
*   At first, follow this link [https://firebase.google.com/](https://firebase.google.com/)
    

![firebase_1](https://docs.retrytech.com/asset/img/doctor/firebase_1.png)

*   Now, we first have to create a Firebase project. Firebase project will go through and describe what it is. This allows us to add an app to that project. It can have many projects inside of Firebase.
    

![firebase_2](https://docs.retrytech.com/asset/img/doctor/firebase_2.png)

*   Now, we have to give a name and id to the project, enable Google Analytics for the project, set an analytics location, and accept all the terms and conditions. Firebase console automatically creates a unique id for the project.
    

*   **Step 1 :** Giving a name to the project
    

![firebase_3](https://docs.retrytech.com/asset/img/doctor/firebase_3.png)

*   **Step 2 :** Enable Google analytics for the project
    

![firebase_4](https://docs.retrytech.com/asset/img/doctor/firebase_4.png)

*   **Step 3 :** First Choose default Firebase account and then create project
    

![firebase_5](https://docs.retrytech.com/asset/img/doctor/firebase_5.png)

![firebase_6](https://docs.retrytech.com/asset/img/doctor/firebase_6.png)

Add Android app to Firebase
===========================

*   In the next step, we have to choose the platform to add Firebase to our application. The platform can be Android, iOS, Web etc..
    

![android_firbase_1](https://docs.retrytech.com/asset/img/doctor/android_firbase_1.png)

*   Your package name is generally the **applicationId** in your **build.gradle (app-level)** file
    
*   [See this page](https://docs.retrytech.com/how_to_get_sha1_key) for information on using keytool to get the **SHA-1** hash of your signing certificate
    
*   Add your **applicationid** in the first field and **SHA-1** to the third field as shown in the image below.
    

![android_firbase_2](https://docs.retrytech.com/asset/img/doctor/android_firbase_2.png)

*   Download the **google-services.json** file & place it in your project's app root directory.
    

![android_firbase_3](https://docs.retrytech.com/asset/img/doctor/android_firbase_3.png)

![android_app](https://docs.retrytech.com/asset/img/android_app.png)

*   Back in the Firebase console-setup workflow, click **Next** to skip the remaining steps and then finish and complete
    

![android_firbase_4](https://docs.retrytech.com/asset/img/doctor/android_firbase_4.png)

Add iOS app in Firebase
=======================

*   We have to choose the platform to add Firebase to our application. Click on iOS.
    

![ios_firbase_1](https://docs.retrytech.com/asset/img/doctor/ios_firbase_1.png)

*   On the next screen, enter your iOS bundle ID & App nickname and click on Register App. You can find your **bundle ID** in the General tab for your app's primary target in Xcode. If specified, the app nickname will be used throughout the Firebase console to represent this app. Nicknames aren't visible to users.
    

![ios_firbase_2](https://docs.retrytech.com/asset/img/doctor/ios_firbase_2.png)

*   Download the GoogleService-Info.plist file & move the GoogleService-Info.plist file you just downloaded into the root of your Xcode project and add it to all targets. Make sure the config file is not appended with additional characters, like (2).
    

![ios_firbase_3](https://docs.retrytech.com/asset/img/doctor/ios_firbase_3.png)

![android_firbase_3](https://docs.retrytech.com/asset/img/doctor/ios_firbase_3_a.png)

*   Back in the Firebase console-setup workflow, click **Next** to skip the remaining steps and the finish.
    

![ios_firbase_4](https://docs.retrytech.com/asset/img/doctor/ios_firbase_4.png)

Email sign in
=============

*   Click to Authentication and sign in mathod tab
    
*   Then click on **email/password** provider
    

![android_firbase_1](https://docs.retrytech.com/asset/img/doctor/auth_1.png)

![android_firbase_1](https://docs.retrytech.com/asset/img/doctor/auth_2.png)

![android_firbase_1](https://docs.retrytech.com/asset/img/sign_in/email_1.png)

*   Then both button switch to enable and save
    

![android_firbase_1](https://docs.retrytech.com/asset/img/sign_in/email_2.png)

*   Your email and password successfully Enable
    

![android_firbase_1](https://docs.retrytech.com/asset/img/sign_in/email_3.png)

Enable firestore
================

*   **Step 1 :** Click on Firestore Database and Create database.
    

![firebase_1](https://docs.retrytech.com/asset/img/doctor/firestore_1.png)

![firebase_1](https://docs.retrytech.com/asset/img/doctor/firestore_2.png)

*   **Step 2 :** Model will be open click on **Next.**
    

![firebase_1](https://docs.retrytech.com/asset/img/doctor/firestore_3.png)

*   **Step 3 :** Then click **Enable** button
    

![firebase_1](https://docs.retrytech.com/asset/img/doctor/firestore_4.png)

*   **Step 4 :** After create Database, You have to change rules of database then click **publish** button. Follow step, shown below.
    

![firebase_1](https://docs.retrytech.com/asset/img/doctor/firestore_5.png)

![firebase_1](https://docs.retrytech.com/asset/img/doctor/firestore_6.png)

*   **Step 5 :** Create index in firestore.
    

![firebase_1](https://docs.retrytech.com/asset/img/doctor/firestore_7.png)

*   **Index**
    

*   Collection ID : **chats**
    
*   Fields :
    
    *   **usersIds** \= Arrays
        
    *   **time** \= Descending
        
*   Query Scope : Select Collection same as below the image.
    

![firebase_1](https://docs.retrytech.com/asset/img/firestore_8_1.png)

*   After completing this index, the result will look like the image below.
    

![firebase_1](https://docs.retrytech.com/asset/img/firestore_10_1.png)

Setup Agora
===========

*   Follow [This guide](https://docs.retrytech.com/agora_project_setup) and setup project at agora and collect **App id**
    
*   Go to your flutter project and Paste Here : **Zync > lib > utilities > const.dart**
    

![firebase_1](https://docs.retrytech.com/asset/img/agaora_flutter_Zync.png)

![firebase_1](https://docs.retrytech.com/asset/img/doctor/agora_8.png)

![firebase_1](https://docs.retrytech.com/asset/img/doctor/agora_9.png)

*   In downloaded file, you will get **customerID** and **customerSecret** keys.
    
*   Please add these to the project file as shown below
    
*   Paste here : **Zync > lib > utilities > const.dart**
    

![firebase_1](https://docs.retrytech.com/asset/img/agaora_flutter_Zync_2.png)

Branch.io Setup
===============

*   Follow [This guide](https://docs.retrytech.com/branch_io) and setup project at Branch.io.
    

Revenuecat
==========

*   **Setup subscriptions**
    

*   You need to define subscriptions on [Google Play Console](https://play.google.com/console/u/0/signup) (For Android) and [Apple App Store Connect](https://appstoreconnect.apple.com/login) (For iOS) before connecting with RevenueCat.
    

Android in App Purchase Setup
=============================

*   **Play Store subscription setup**
    

*   For configuring subscriptions on Google Play Console, follow the steps below:
    

*   Go to [Google Play Console](https://play.google.com/console/u/0/signup) . Log in with your developer account.
    
*   Select the app in which you want to add subscriptions.
    
*   From the left menu, under the Monetize section, expand the Products category. Select Subscriptions.
    

![RC1](https://docs.retrytech.com/asset/img/RC1.png)

*   **Let's start creating the subscriptions:**
    

*   From the Monetize > Products > Subscriptions page, click **Create subscription.**
    
*   Select the app in which you want to add subscriptions.
    
*   From the left menu, under the Monetize section, expand the Products category. Select Subscriptions.
    

![RC1](https://docs.retrytech.com/asset/img/RC2.png)

*   Enter a unique **Product ID** for your subscription and a publicly viewable **Name.** Click **Create.**
    
*   For example, we will be creating a subscription for 3 months with:
    

*   **Product ID:** test\_3m
    
*   **Name:** Premium - 3 Months
    

Note : You won't be able to change or reuse a Product ID across any of your apps, even if the product is deleted.

![RC1](https://docs.retrytech.com/asset/img/RC3.png)

*   Click "**Add a base plan**"
    

![RC1](https://docs.retrytech.com/asset/img/RC4.png)

*   Enter the **Base plan ID, Renewal type** (RevenueCat supports only Auto-renewing), **Tags , and Price.** Click Save.
    

![RC1](https://docs.retrytech.com/asset/img/RC5.png)

*   Click **Activate**
    

![RC1](https://docs.retrytech.com/asset/img/RC6.png)

*   Similarly, add two more subscriptions for **6 months and 12 months** .
    

![RC1](https://docs.retrytech.com/asset/img/RC7.png)

*   That completes the subscription setup for the Google Play Console. Let's move on to the play Store subscription setup.
    

iOS in App Purchase Setup
=========================

**Before making products, Let's agree Agreements**

*   Open [App Store Connect](https://appstoreconnect.apple.com/apps/) And select your app.
    
*   Note : Make you have agreed and added bank details at [Agreements](https://appstoreconnect.apple.com/agreements/#/)
    

![firebase_1](https://docs.retrytech.com/asset/img/in_app_purchase_13.png)

*   Once you agree this, both status should be active like this
    

![firebase_1](https://docs.retrytech.com/asset/img/in_app_purchase_14.png)

#### **App Store subscription setup**

*   Follow the steps below to configure subscriptions on App Store Connect:
    

*   Go to [App Store Connect](https://appstoreconnect.apple.com/login) and log in with your developer account.
    
*   Select the **App**
    

![RC1](https://docs.retrytech.com/asset/img/RC8.png)

*   Choose the app in which your want to add subscriptions.
    

![RC1](https://docs.retrytech.com/asset/img/RC9.png)

*   Select **Subscriptions** from the left menu and click **Create** under **Subscription Groups.**
    

![RC1](https://docs.retrytech.com/asset/img/RC10.png)

*   Enter a name for the Subscription Group and click **Create**.
    

Learn in detail about iOS Subscription Groups [**here**](https://www-origin.revenuecat.com/blog/engineering/ios-subscription-groups-explained/) .

![RC1](https://docs.retrytech.com/asset/img/RC11.png)

*   This will create and open the Subscription Group. From this page, you will be able to create subscriptions for your app. Click **Create** under **Subscriptions** .
    

![RC1](https://docs.retrytech.com/asset/img/RC12.png)

*   Enter a **Reference Name** and **Product ID** for the subscription. Use the same format for the Product ID as we had described earlier. Click **Create** .
    

![RC1](https://docs.retrytech.com/asset/img/RC13.png)

*   This will take you to the subscription details page. Select the **Subscription Duration** .
    

![RC1](https://docs.retrytech.com/asset/img/RC14.png)

*   Scroll down to the **Subscription Prices** section and click "**Add Subscription Price**" button.
    

![RC1](https://docs.retrytech.com/asset/img/RC15.png)

*   Enter the subscription price in your preferred currency. Click **Next**.
    

![RC1](https://docs.retrytech.com/asset/img/RC16.png)

*   The next page will show you the automatically calculated prices for other countries and regions. Click **Next**.
    

![RC1](https://docs.retrytech.com/asset/img/RC17.png)

*   Click Confirm on the next page.
    

![RC1](https://docs.retrytech.com/asset/img/RC18.png)

*   Scroll down to the **App Store Localization** section. Click "**Add Localization**".
    

![RC1](https://docs.retrytech.com/asset/img/RC19.png)

*   Select your preferred language and enter a **Display Name** and **Description** . Click **Add** .
    

![RC1](https://docs.retrytech.com/asset/img/RC20.png)

*   You can skip the **App Store Promotion** for now as it's optional.
    

![RC1](https://docs.retrytech.com/asset/img/RC21.png)

*   Under the **Review Information** section, add a screenshot of the subscription screen of your app (you can also add a blank screenshot, having proper size for now, if you haven't yet created the subscription UI).
    

![RC1](https://docs.retrytech.com/asset/img/RC22.png)

*   Scroll up to the top of the subscription page, and click Save. You will see a warning message if you haven't yet added localization to your subscription group. Click **Add localizations** (skip if you have already added).
    

![RC1](https://docs.retrytech.com/asset/img/RC23.png)

*   This will take you back to the subscription group page. Click **Create** under **App Store Localization.**
    

![RC1](https://docs.retrytech.com/asset/img/RC24.png)

*   Select your preferred language, enter a **Subscription Group Display Name**, and **select App Name.** Click **Create** .
    

![RC1](https://docs.retrytech.com/asset/img/RC25.png)

*   This completes the addition of a subscription. You can follow similar steps for adding the other subscription plans as well, use the plus **("+")** button next to **Subscriptions** .
    

![RC1](https://docs.retrytech.com/asset/img/RC26.png)

*   With all the subscription plans defined on Play Console and App Store Connect, we are ready to connect with RevenueCat.
    

* * *

### **Connect with RevenueCat**

*   Create an account or log in to RevenueCat from [here](https://www.revenuecat.com/?utm_medium=referral&utm_source=techp&utm_campaign=flutterflow&utm_content=partner) to get started.
    

![RC1](https://docs.retrytech.com/asset/img/RC27.png)

*   If you have created a new account, you will be automatically prompted to create your first project. Enter a **Project name** and click **"CREATE PROJECT"** button.
    

![RC1](https://docs.retrytech.com/asset/img/RC28.png)

*   Next, you need to add your Android and iOS apps to RevenueCat in order to use and manage the subscriptions.
    

### **Adding Android app**

*   Let's start by configuring the Android app:
    

*   Go to **Apps** under **Project settings** (from the left menu). Select **Play Store** .
    

![RC1](https://docs.retrytech.com/asset/img/RC29.png)

*   Enter the **App name** and the **package ID.**
    

![RC1](https://docs.retrytech.com/asset/img/RC30.png)

*   You need to create another **Service Account** for RevenueCat. Follow [This guide](https://www.revenuecat.com/docs/creating-play-service-credentials?utm_medium=referral&utm_source=techp&utm_campaign=flutterflow&utm_content=partner) to generate the credentials in JSON format. Drag and drop the **Credentials JSON** file. Click **"SAVE CHANGES".**
    

![RC1](https://docs.retrytech.com/asset/img/RC31.png)

*   This completes the Android app setup on RevenueCat.
    

### **Adding iOS app**

*   Follow the steps below to configure the iOS app:
    

*   Go back to the Apps page and click on "+ New".
    

![RC1](https://docs.retrytech.com/asset/img/RC32.png)

*   Select **App Store.**
    

![RC1](https://docs.retrytech.com/asset/img/RC33.png)

*   Enter an App name, Bundle ID, and App-Specific Shared Secret. To generate an App-Specific Shared Secret, follow [The guide](https://www.revenuecat.com/docs/itunesconnect-app-specific-shared-secret?utm_medium=referral&utm_source=techp&utm_campaign=flutterflow&utm_content=partner) . Once you have the key, click "SET SECRET", enter the value, and click Set. Then click "SAVE CHANGES".
    

![RC1](https://docs.retrytech.com/asset/img/RC34.png)

*   This completes the iOS app setup on RevenueCat.
    

### **Define subscriptions on RevenueCat**

*   You will find these configuration levels on the left menu of the RevenueCat dashboard under the section **Product Setup:**
    

![RC1](https://docs.retrytech.com/asset/img/RC35.png)

### **Products**

*   In this configuration, you need to add all the subscriptions for both your Android and iOS app that the user can purchase. This is like a 1-to-1 mapping of the products in RevenueCat that you have already added to the stores (Google Play Store and Apple App Store).
    
*   To add products, follow these steps:
    
*   Select **Products** under the Product Setup section. Click **"+ New".**
    

![RC1](https://docs.retrytech.com/asset/img/RC36.png)

*   You need to enter the product **Identifier** and the **App** . Make sure you use exactly the same product ID you used for the Android/iOS subscription. Click **ADD** .
    

![RC1](https://docs.retrytech.com/asset/img/RC37.png)

*   Similarly, add the other subscriptions as well (for both Android and iOS).
    

![RC1](https://docs.retrytech.com/asset/img/RC38.png)

### **Entitlements**

*   Follow these steps to add an entitlement:
    

*   Select **Entitlements** under the Product Setup section. Click **"+ New".**
    

![RC1](https://docs.retrytech.com/asset/img/RC39.png)

*   Enter an **Identifier** and **Description** for the entitlement. Click **ADD.**
    

![RC1](https://docs.retrytech.com/asset/img/RC40.png)

*   Next, you need to attach the products to this entitlement. Click on the entitlement that you just created.
    

![RC1](https://docs.retrytech.com/asset/img/RC41.png)

*   Click on **Attach.**
    

![RC1](https://docs.retrytech.com/asset/img/RC42.png)

*   Select a **Product** from the dropdown and click **ADD .**
    

![RC1](https://docs.retrytech.com/asset/img/RC43.png)

*   Similarly, attach all the other products to this entitlement.
    

![RC1](https://docs.retrytech.com/asset/img/RC44.png)

### **Offerings**

*   Follow the steps below to add offerings:
    

*   Select **Offerings** under the Product Setup section. Click **"+ New".**
    

![RC1](https://docs.retrytech.com/asset/img/RC45.png)

*   Enter an **Identifier** and **Description** for the offering. Click **ADD.**
    

![RC1](https://docs.retrytech.com/asset/img/RC46.png)

*   Click to open the offering that you just created.
    

![RC1](https://docs.retrytech.com/asset/img/RC47.png)

*   Click on **"+ New"** beside the Packages.
    

![RC1](https://docs.retrytech.com/asset/img/RC48.png)

*   Enter an **Identifier** for the package from the dropdown and add a **Description** . Click **ADD.**
    

![RC1](https://docs.retrytech.com/asset/img/RC49.png)

*   Similarly, add the other packages as well.
    

![RC1](https://docs.retrytech.com/asset/img/RC50.png)

*   Click to open a package. Then click Attach.
    

![RC1](https://docs.retrytech.com/asset/img/RC51.png)

*   Select the respective Play Store and App Store products from the dropdown. Click **Attach.**
    

![RC1](https://docs.retrytech.com/asset/img/RC52.png)

*   Similarly, attach the correct products to the other two packages as well.
    

![RC1](https://docs.retrytech.com/asset/img/RC53.png)

*   This completes the three levels of configuration on the RevenueCat.
    

### **RevenueCat Project setup**

*   you need to add the App Store Key and Play Store Key to Your project You can get these keys by going to the RevenueCat dashboard > API Keys > Public app-specific API keys. Copy and paste these keys into the respective fields of Project
    

![RC1](https://docs.retrytech.com/asset/img/RC55.png)

![RC1](https://docs.retrytech.com/asset/img/RC54.png)

![RC56](https://docs.retrytech.com/asset/img/RC57.png)

Google Admob
============

*   Open [https://admob.google.com/home/get-started/](https://admob.google.com/home/get-started/) URL and setup account.
    
*   After configuring Ads in your admob consol, you have to add ad\_ids accordingly in your admin panel.
    

![payment_1](https://docs.retrytech.com/asset/img/Zync_admob.png)

Create application build
========================

*   Follow [This guide](https://docs.flutter.dev/deployment/android) and you can create build for android.
    
*   Follow [This guide](https://docs.flutter.dev/deployment/ios) and you can create build for iOS.
    

Update info
===========

*   To upgrade your project, you have to **Add/Update/Remove files.** Please check below file for the information.
    
*   File name : **README.md**
    
*   Please be careful while making an updates this way, It might result in errors sometimes.
    
*   If it comes any issues while making an update, you are absolutely responsible for that since updating existing project is not included in the support.
    

Want to talk with us?
---------------------

*   Telegram (Support Desk) : [+91 7070799200](https://t.me/+917070799200)
*   Email : [sudhirkdnw@gmail.com](mailto:sudhirkdnw@gmail.com)
*   Whatsapp (No Support Here) : [+91 7070799200](https://wa.me/7070799200)

$(window).scroll(function() { if ($(window).scrollTop() + $(window).height() == $(document).height()) { $('.nav-item').removeClass('active'); $('.nav-item .nav-link').removeClass('active'); $('.nav-item:last-child').addClass('active'); } else { $('.nav-item:last-child').removeClass('active'); } });