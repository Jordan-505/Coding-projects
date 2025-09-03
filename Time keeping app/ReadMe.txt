NAME: Chrono works (timesheet app)
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

-You will need aa android device with android 7 or higher
-at least 2 GB of storage

=================================================================================== 
3
FAQs:

Q:1
if I don't create a category first when making a task. will it automatically make one for me?
A:1
No you will first need to make a category so a task can be assigned to that category

Q:2
Will I be able to fetch all tasks?
A:2
Yes. if you don't select a date to fetch tasks between it will fetch all tasks.

===================================================================================
4
Developer info:

ST10047883
st10047883@vcconnect.edu.za
Jordan Joel Reddy
=================================================================================== 
5
Framework and Plugins:

android {
    namespace 'com.example.opsc_part_2'
    compileSdk 34

    defaultConfig {
        applicationId "com.example.opsc_part_2"
        minSdk 27
        targetSdk 34
        versionCode 1
        versionName "1.0"

        testInstrumentationRunner "androidx.test.runner.AndroidJUnitRunner"
    }

dependencies {

    implementation 'androidx.core:core-ktx:1.7.0'
    implementation 'androidx.appcompat:appcompat:1.6.1'
    implementation 'com.google.android.material:material:1.11.0'
    implementation 'androidx.constraintlayout:constraintlayout:2.1.4'
    implementation 'androidx.lifecycle:lifecycle-livedata-ktx:2.7.0'
    implementation 'androidx.lifecycle:lifecycle-viewmodel-ktx:2.7.0'
    implementation 'androidx.navigation:navigation-fragment-ktx:2.7.7'
    implementation 'androidx.navigation:navigation-ui-ktx:2.7.7'

    implementation 'com.google.firebase:firebase-auth:22.3.1'
    implementation 'com.google.firebase:firebase-database:20.3.1'

    implementation "androidx.recyclerview:recyclerview:1.2.1"
    implementation 'com.google.firebase:firebase-storage-ktx:20.3.0'
    implementation 'com.google.firebase:firebase-firestore-ktx:24.11.1'

    implementation 'com.github.bumptech.glide:glide:4.12.0'
    annotationProcessor 'com.github.bumptech.glide:compiler:4.12.0'

    testImplementation 'junit:junit:4.13.2'
    androidTestImplementation 'androidx.test.ext:junit:1.1.5'
    androidTestImplementation 'androidx.test.espresso:espresso-core:3.5.1'
}
=================================================================================== 
6
Update Report:

The program has been made so that it now meets the requirements.

The programs layout and design have been altered from the original part 1 design
to help better compensate for user accessability.

A dual graident background has been added to make the application more appealing.
=================================================================================== 
7
code attributions:

https://console.firebase.google.com/u/0/project/opsc-part-2-82f81/database/opsc-part-2-82f81-default-rtdb/data (Accessed: May 1, 2024).
https://uizard.io/blog/guide-to-designing-ui-mockups/ (Accessed: April 21, 2024).
=================================================================================== 
8
Links:
https://github.com/VCWVL/opsc7311---open-source-coding---poe-ST10047883.git
=================================================================================== 
9
My features:
for my first feature I have included a drop down when creating a task that allows the user to set the status of the task
to: TO DO, IN PROGGRES, DONE.

for the second feature I have included a due date option the allows the user to set when the task is due.
