# Unity Android Library Project Template

> Dev Version 0.1.0

> Suggist Unity Android Project Export Path : `YourUnityProjectFolder/Build/Android`

## Step

1. Make Unity Project
2. Download this Template
3. Put it to Assets/Plugins/Android Path
4. Rename Root Folder to "xxxxx.androidlib"
5. Select xxxxx.androidlib in Unity
6. Check Unity Inspector ,Change "Select dependent module" to None
7. Open Unity BuildProfile Panel, Export Android Project
8. Run Android Project in Android Studio
9. Edit your Android Lib
10. Execute MCopyAndroidLibToUnity Update UnityProject File




## Tools

Auto Copy AndroidLib To Unity

In build.gradle script :

```groovy
task MCopyAndroidLibToUnity(type: Copy) 
{
    from '../UnityAndroidLibTemplate.androidlib'
    into '../../../Assets/Plugins/Android/UnityAndroidLibTemplate.androidlib'
}
```

