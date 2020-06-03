This fork removes the team and sharing features from v3.1.1, reducing the total number of methods from 37537 to 8057(without proguard) and 833(with proguard). You can use it in applications that only need to access the App folder.

#### dropbox-core-sdk:3.1.1 without proguard:
```
methods  fields   package/class name
37537    9622     com.dropbox
37537    9622     com.dropbox.core
74       69       com.dropbox.core.android
196      83       com.dropbox.core.http
122      36       com.dropbox.core.json
43       26       com.dropbox.core.oauth
133      22       com.dropbox.core.stone
176      28       com.dropbox.core.util
390      210      com.dropbox.core.v1
36022    8979     com.dropbox.core.v2
125      29       com.dropbox.core.v2.async
234      66       com.dropbox.core.v2.auth
8        1        com.dropbox.core.v2.callbacks
138      32       com.dropbox.core.v2.common
59       13       com.dropbox.core.v2.contacts
1004     271      com.dropbox.core.v2.fileproperties
505      174      com.dropbox.core.v2.filerequests
4237     1124     com.dropbox.core.v2.files
969      262      com.dropbox.core.v2.paper
19       11       com.dropbox.core.v2.seenstate
4583     1497     com.dropbox.core.v2.sharing
4674     1349     com.dropbox.core.v2.team
108      36       com.dropbox.core.v2.teamcommon
18612    3865     com.dropbox.core.v2.teamlog
270      83       com.dropbox.core.v2.teampolicies
348      109      com.dropbox.core.v2.users
19       6        com.dropbox.core.v2.userscommon
```

#### This fork without proguard:
```
methods  fields   package/class name
8057     2452     com.dropbox
8057     2452     com.dropbox.core
74       69       com.dropbox.core.android
196      83       com.dropbox.core.http
122      36       com.dropbox.core.json
43       26       com.dropbox.core.oauth
133      22       com.dropbox.core.stone
176      28       com.dropbox.core.util
390      210      com.dropbox.core.v1
6542     1809     com.dropbox.core.v2
37       10       com.dropbox.core.v2.async
234      66       com.dropbox.core.v2.auth
8        1        com.dropbox.core.v2.callbacks
138      32       com.dropbox.core.v2.common
59       13       com.dropbox.core.v2.contacts
988      268      com.dropbox.core.v2.fileproperties
505      174      com.dropbox.core.v2.filerequests
4125     1093     com.dropbox.core.v2.files
343      106      com.dropbox.core.v2.users
19       6        com.dropbox.core.v2.userscommon
```

#### With proguard:
```
methods  fields   package/class name
833      557      com.dropbox
833      557      com.dropbox.core
30       34       com.dropbox.core.android
63       47       com.dropbox.core.http
22       13       com.dropbox.core.json
14       15       com.dropbox.core.oauth
60       14       com.dropbox.core.stone
40       10       com.dropbox.core.util
0        1        com.dropbox.core.v1
517      357      com.dropbox.core.v2
0        1        com.dropbox.core.v2.async
60       39       com.dropbox.core.v2.auth
1        0        com.dropbox.core.v2.callbacks
61       26       com.dropbox.core.v2.common
0        1        com.dropbox.core.v2.contacts
65       53       com.dropbox.core.v2.fileproperties
0        8        com.dropbox.core.v2.filerequests
308      201      com.dropbox.core.v2.files
0        2        com.dropbox.core.v2.users
```


### Building from source

```
git clone https://github.com/qmonk/dropbox-sdk-java
cd dropbox-sdk-java
./update-submodules
./gradlew build
```


