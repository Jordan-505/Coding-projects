NAME: Cheshire Home website and app
=================================================================================== 
INDEX:

1 - Version
2 - Hardware Specs
3 - FAQs
4 - Developer info
5 - Framework and Plugins
6 - code attributions 
7 - Links
8 - My features and updates
9 - Important note
=================================================================================== 
1
Version:

<?xml version="1.0" encoding="utf-8" ?>
=================================================================================== 
2
Hardware Specs:

-You will need at least visual studios 2022
-8GB of RAM 
-i3 intel/Ryzen 3 processor
-40GB available storage for visual studios 2022

-You will need an android device with android 7 or higher
-at least 2 GB of storage

=================================================================================== 
3
FAQs:

Q:1
Can I log into the app?

A:1
No. only admins can login same goes for the website.

Q:2
can I make donations on the app/website?

A:2
No. only the details to make a donation are on the app/website.

===================================================================================
4
Developer info:

ST10047883
st10047883@vcconnect.edu.za
Jordan Joel Reddy
=================================================================================== 
5
Framework and Plugins:

<configuration>
    <startup> 
        <supportedRuntime version="v4.0" sku=".NETFramework,Version=v4.7.2" />
    </startup>
</configuration>


APP:
Framework and Plugins:
plugins {
    alias(libs.plugins.androidApplication)
    alias(libs.plugins.jetbrainsKotlinAndroid)
    kotlin("kapt")
    id("com.google.gms.google-services")
}

android {
    namespace = "com.jreddy.opsc_sem_2"
    compileSdk = 34

    bundle {
        language {
            enableSplit = false
        }
    }

    defaultConfig {
        applicationId = "com.jreddy.opsc_sem_2"
        minSdk = 27
        targetSdk = 34
        versionCode = 3
        versionName = "3.0"

        testInstrumentationRunner = "androidx.test.runner.AndroidJUnitRunner"
    }

    buildFeatures{
        viewBinding = true
    }

    buildTypes {
        release {
            isMinifyEnabled = false
            proguardFiles(
                getDefaultProguardFile("proguard-android-optimize.txt"),
                "proguard-rules.pro"
            )
        }
    }
    compileOptions {
        sourceCompatibility = JavaVersion.VERSION_1_8
        targetCompatibility = JavaVersion.VERSION_1_8
    }
    kotlinOptions {
        jvmTarget = "1.8"
    }
    buildFeatures {
        viewBinding = true
    }
}

dependencies {

    implementation(libs.androidx.core.ktx)
    implementation(libs.androidx.appcompat)
    implementation(libs.material)
    implementation(libs.androidx.constraintlayout)
    implementation(libs.androidx.lifecycle.livedata.ktx)
    implementation(libs.androidx.lifecycle.viewmodel.ktx)
    implementation(libs.androidx.navigation.fragment.ktx)
    implementation(libs.androidx.navigation.ui.ktx)
    implementation(libs.firebase.auth)
    implementation(libs.androidx.activity)
    implementation(libs.firebase.database)
    implementation(libs.firebase.firestore)
    implementation(libs.androidx.room.common)
    implementation(libs.androidx.room.ktx)
    implementation(libs.firebase.messaging.ktx)
    implementation(libs.firebase.messaging)
    implementation(libs.core.ktx)
    testImplementation(libs.junit)
    androidTestImplementation(libs.androidx.junit)
    androidTestImplementation(libs.androidx.espresso.core)

    implementation ("com.google.code.gson:gson:2.9.1")
    implementation ("com.squareup.retrofit2:retrofit:2.9.0")
    implementation ("com.squareup.retrofit2:converter-gson:2.9.0")
    implementation ("com.github.bumptech.glide:glide:4.14.2")
    implementation ("com.squareup.okhttp3:okhttp:4.9.3")
    implementation ("androidx.recyclerview:recyclerview:1.3.0")
    implementation ("androidx.appcompat:appcompat:1.6.1")
    implementation ("com.google.android.gms:play-services-auth:20.7.0")
    implementation ("androidx.biometric:biometric:1.2.0-alpha04")

    testImplementation ("junit:junit:4.13.2")
    testImplementation ("org.mockito:mockito-core:3.11.2")
    testImplementation ("org.jetbrains.kotlinx:kotlinx-coroutines-test:1.6.0")
    testImplementation ("androidx.arch.core:core-testing:2.1.0")
    testImplementation ("com.squareup.retrofit2:retrofit-mock:2.9.0")
    implementation ("androidx.lifecycle:lifecycle-runtime-ktx:2.4.1")

    implementation ("com.google.android.gms:play-services-auth:20.3.0")


    implementation ("androidx.room:room-runtime:2.5.0")
    kapt("androidx.room:room-compiler:2.6.1")


=================================================================================== 
6
code attributions:
Needle, F. (2023) The Benefits of Customer Feedback, According to Experts, HubSpot. Available at: https://blog.hubspot.com/service/benefits-of-customer-feedback (Accessed: November 15, 2024).
Personalisation has a huge impact on customer engagement (no date) Ftstrategies.com. Available at: https://www.ftstrategies.com/en-gb/insights/personalisation-has-a-huge-impact-on-customer-engagement-how-mature-are-your-capabilities/ (Accessed: Accessed: November 15, 2024).
ConnexAI (no date) Connex.ai. Available at: https://athena.connex.ai/za/athena-2.0.php?gad_source=1&gclid=Cj0KCQiAouG5BhDBARIsAOc08RRCrNnaE6MpcJyXwUPc98ZG0l1WXVNgLY-5C-Hvp07B7cIwEMnb1moaAsLAEALw_wcB (Accessed: November 16, 2024).
Convert Website to a Progressive Web App: Is It Worth it? (2023) Gomage. Available at: https://www.gomage.com/blog/convert-website-to-progressive-web-app/ (Accessed: November 16, 2024).

=================================================================================== 
7
Links:
https://github.com/ST10047883/WILLS-Project-Cheshire-Home-App-and-website.git

=================================================================================== 
8
My features and updates:
all features and requirements were met per the npo's request

=================================================================================== 
9
Important note:
the app is not on the google play store and is a
internal organization app

Only the mobile apps documentation is provide per the options provided by the WIls
coordinator.
=================================================================================== 