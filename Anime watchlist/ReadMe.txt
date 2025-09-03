NAME: Zero watch (anime watch list)
=================================================================================== 
INDEX:

1 - Version
2 - Hardware Specs
3 - FAQs
4 - Developer info
5 - Framework and Plugins
6 - Update Report
7 - code attributions 
8 - Links
9 - My features
=================================================================================== 
1
Version:

<?xml version="1.0" encoding="utf-8"?>
=================================================================================== 
2
Hardware Specs:

-You will need an android device with android 7 or higher
-at least 2 GB of storage

=================================================================================== 
3
FAQs:

Q:1
How do i delete anime from my list?
A:1
Go to you "To watch' or "watched" and hold down on an anime you want to delete, you will then
be prompted to delete the anime from your list.

Q:2
Will the application save each my anime list per separate account? 
A:2
Yes the application will save each anime list per account separately.

Q:2
Will I be able to use google login when my app is set to Afrikaans? 
A:2
No, for an unknown reason when you log out while the language is set to Afrikaans, you won't be able 
to use the google log in.

===================================================================================
4
Developer info:

ST10047883
st10047883@vcconnect.edu.za
Jordan Joel Reddy
=================================================================================== 
5
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

}=================================================================================== 
6
Update Report:

The program has been made so that it now meets the requirements discussed in part 3.

The programs layout and design have been altered from the original part 1 and 2 design
to help better compensate for user accessibility.

An API has been implemented in the application as well as real-time notification and language changing accessibility

PS. Language will reset if the application is closed. Language will become buggy at times
=================================================================================== 
7
code attributions:

https://console.firebase.google.com/u/0/project/opsc-sem-2-c6a09/overview (Accessed: September 1, 2024).
https://uizard.io/blog/guide-to-designing-ui-mockups/ (Accessed: September 1, 2024).
=================================================================================== 
8
Links:
https://github.com/VCWVL/opsc7312-poe-ST10047883.git
=================================================================================== 
9
My features:
User list: the user is able to add different anime to their own individual list and
change it from watch/ plan to watch list, delete anime from their list, by holding down on the anime 

Top anime: The user is be able to view different top rated anime based on the
categories of: all, airing, upcoming, tv, ova, movie, special and popularity.

Search function: user is able to search for different anime's.
