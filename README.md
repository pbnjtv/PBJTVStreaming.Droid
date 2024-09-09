# PBJTVStreaming.Droid
0.  PREREQUISITE: Minimum supported SDK must be at least 26
1. Download the AAR from the latest release of the SDK
2. Include the AAR in your projects directory
3. Within Android Studio, access the File > Project Structure menu
4. Go to the ‘Dependencies’ tab.
5. Choose your app’s module from the ‘Modules’ panel, then from the ‘Declared Dependencies’ panel, click the + sign, then ‘JAR/AAR Dependency’
6. Enter the path to the AAR in the first field. The second field needs to be set to ‘Implementation’, after which you can add the dependency. 
7. Open your build.gradle (or build.gradle.kts for Kotlin projects). You’ll need to add several dependencies, after which you can sync your gradle files and then build the application again. I’ve added them below in the Kotlin format:

```
implementation("androidx.core:core-ktx:1.12.0")
implementation("androidx.appcompat:appcompat:1.6.1")
implementation("com.google.android.material:material:1.11.0")
implementation("androidx.lifecycle:lifecycle-runtime-ktx:2.7.0")
implementation("androidx.activity:activity-compose:1.8.2")
implementation(platform("androidx.compose:compose-bom:2023.08.00"))
implementation("androidx.compose.ui:ui")
implementation("androidx.compose.ui:ui-graphics")
implementation("androidx.compose.ui:ui-tooling-preview")
implementation("androidx.compose.material3:material3")
implementation("com.squareup.picasso:picasso:2.8")
implementation("com.squareup.retrofit2:retrofit:2.9.0")
implementation("com.squareup.retrofit2:converter-gson:2.9.0")
implementation("androidx.fragment:fragment-ktx:1.7.1")
implementation("androidx.navigation:navigation-fragment-ktx:2.7.7")
implementation("androidx.navigation:navigation-ui-ktx:2.7.7")
implementation("androidx.media3:media3-exoplayer:1.3.1")
implementation("androidx.media3:media3-ui:1.3.1")
implementation("androidx.media3:media3-exoplayer-hls:1.3.1")
```


