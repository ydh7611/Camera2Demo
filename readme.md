#### Camera2Demo
1.演示Camera2的使用

2.获取预览帧数据并隔一段时间将原始画面和处理过的画面显示到UI上

3.将预览的YUV数据转换为NV21，再转换为Bitmap并显示到控件上，同时也将该Bitmap转换为相机预览效果的Bitmap显示到控件上，便于了解原始数据和预览画面的关系

![demo演示](https://github.com/wangshengyang1996/Camera2Demo/blob/master/sample.png)


修改以下内容，可解决导入时，包出错问题。
compileSdkVersion 30

targetSdkVersion 30
由28改为30

dependencies {
    def appcompat_version = "1.2.0"

    implementation "androidx.appcompat:appcompat:$appcompat_version"
    // For loading and tinting drawables on older versions of the platform
    implementation "androidx.appcompat:appcompat-resources:$appcompat_version"
    implementation fileTree(dir: 'libs', include: ['*.jar'])
//    implementation 'androidx.appcompat:appcompat:1.0.2'
//    implementation 'androidx.appcompat:appcompat:1.2.0'
    implementation 'androidx.constraintlayout:constraintlayout:1.1.3'
    testImplementation 'junit:junit:4.12'
    androidTestImplementation 'androidx.test:runner:1.2.0'
    androidTestImplementation 'androidx.test.espresso:espresso-core:3.2.0'
}

distributionUrl=https\://services.gradle.org/distributions/gradle-6.7.1-all.zip
