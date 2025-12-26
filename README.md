# Important Uri Link

### Website URI
```
final Uri _websiteUri = Uri.parse("https://flutter.dev");
```

### Phone call URI

##### Manifest
```
    <queries>
        <intent>
            <action android:name="android.intent.action.DIAL"/>
            <data android:scheme="tel"/>
        </intent>
    </queries>
```
##### url_launcher package install

#### Function
```
Future<void> makePhoneCall(String phone) async {
  final Uri launchUri = Uri(scheme: 'tel', path: phone);

  if (await canLaunchUrl(launchUri)) {
    await launchUrl(launchUri);
  } else{
    debugPrint('Could not launch $phone');
  }
}
```

#### OnPress
```
onPressed: () {makePhoneCall(phone);},
```

### Email URI
```
final Uri _emailUri = Uri(
  scheme: 'mailto',
  path: 'example@email.com',
  query: 'subject=Hello&body=This is a test email',
);
```

### Go to Whatsapp

```
https://wa.me/+880
```


### Go to Massenger

```
https://m.me/0xfaysal
```


### Youtube Thumbnil Link

```
https://img.youtube.com/vi/<insert-youtube-video-id-here>/0.jpg

https://img.youtube.com/vi/<insert-youtube-video-id-here>/1.jpg

https://img.youtube.com/vi/<insert-youtube-video-id-here>/2.jpg

https://img.youtube.com/vi/<insert-youtube-video-id-here>/3.jpg
```


###### © All right reserved by Faysal


