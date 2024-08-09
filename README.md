# 0. NOTE IMPORTANT

Run command line: Dùng để dọn sạch cache sau khi cài đặt các package tại mục **#1**

- cd vào folder android

```bash
cd ./android
```

```bash
./gradlew clean
```

# 1. Config with ANDROID

## 1.1. Config MODE "portrait" [AndroidManifest.xml](android/app/src/main/AndroidManifest.xml)

(Helpter: App chỉ hoạt động ở chế độ đọc <mode: portrait> không bị xoay )

```xml
      <activity
        android:name=".MainActivity"
        android:label="@string/app_name"
    +   android:screenOrientation="portrait"
        android:configChanges="keyboard|keyboardHidden|orientation|screenLayout|screenSize|smallestScreenSize|uiMode"
        android:launchMode="singleTask"
        android:windowSoftInputMode="adjustResize"
        android:exported="true">
        <intent-filter>
            <action android:name="android.intent.action.MAIN" />
            <category android:name="android.intent.category.LAUNCHER" />
        </intent-filter>
      </activity>
```

## 1.2. Các thư viện sử dụng chính

- **@react-navigation/native** : dùng điều hướng qua các màn [Documents](https://reactnavigation.org/docs/getting-started)

Các package **react-native-screens**, **react-native-safe-area-context** : là các gói phụ liên quan đến màn hình

```bash
npm install @react-navigation/native react-native-screens react-native-safe-area-context

```

- **@react-navigation/bottom-tabs** : dùng tạo Bottom Tabs Navigator [Documents](https://reactnavigation.org/docs/tab-based-navigation)

```bash
npm install @react-navigation/bottom-tabs

```

- **@react-native-async-storage/async-storage** : dùng lưu trữ các giá trị bất đồng bộ, không mã hóa [Documents](https://www.npmjs.com/package/@react-native-async-storage/async-storage)

```bash
npm i @react-native-async-storage/async-storage

```

- **zustand** : dùng quản lý state global [Documents](https://www.npmjs.com/package/zustand)

```bash
npm i zustand

```

- **lottie-react-native** : Tạo hoạt ảnh animations [Documents](https://www.npmjs.com/package/lottie-react-native)

```bash
npm i lottie-react-native

```

- **react-native-vector-icons** : icons [Documents](https://github.com/oblador/react-native-vector-icons)

```bash
npm install --save react-native-vector-icons

```

- **react-native-linear-gradient** : Tạo Background Linear Gradient [Documents](https://www.npmjs.com/package/react-native-linear-gradient)

```bash
npm i react-native-linear-gradient

```

- **@react-native-community/blur** : Tạo Background blur [Documents](https://www.npmjs.com/package/@react-native-community/blur)

```bash
npm i @react-native-community/blur

```

# 2. Structure Folder Project
