
# Resource obfuscated apk decompiling tool
## Modified from Apktool
* Decompiles almost all resource obfuscated apks (like wechat, tiktok) ...
* Decompiles splitted apks
* Renames illegal names like @layout/aa -> @layout/layout_0a12
* Modified aapt binary tool (for now linux only) to handle illegal character java class names
* Nicely indented xml

## Downloads 
* [Prebuilt jar file ](../master/bin/kikfox.jar)
* [Jar](https://raw.githubusercontent.com/kikfox/kikfox/main/bin/kikfox.jar)
* [Sample decompiled (tiktok 20.0.3)](https://mega.nz/file/VnoEmIQL#TQhMPLPk9ZyDkc6GV_YrmkWAjSoHejqdBR5zHJ2d-2c)
## Source code
* Coming soon
## How to decompile/recompile
* Same as apktool
```console
d@d-TEC:~/kikfox$ java -jar Kikfox.jar "d" "-p" "/home/d/apktool/framework" "-o" "/home/d/kikfox/tiktok_decompiled" "/home/d/kikfox/tiktok_20"
I: Using kikfox 2.4.0 on [23] apk files BASE APK=base.apk
      1) base.apk             2) config.th.apk        3) config.arm64_v8a.apk
      4) config.hi.apk        5) config.ja.apk        6) config.en.apk       
      7) config.zh.apk        8) config.ru.apk        9) config.es.apk       
     10) config.de.apk       11) config.in.apk       12) config.ko.apk       
     13) config.ar.apk       14) config.xxxhdpi.apk  15) config.my.apk       
     16) config.it.apk       17) config.pt.apk       18) config.tr.apk       
     19) df_photomovie.apk   20) df_fusing.apk       21) config.id.apk       
     22) config.fr.apk       23) config.vi.apk       

I:    Loading resource table  'base.apk'
I:    Loading resource table  'config.th.apk'
I:    Loading resource table  'config.arm64_v8a.apk'
W:       No resource table found in: 'config.arm64_v8a.apk'
        ERROR=Could not load resources.arsc from file: config.arm64_v8a.apk
I:    Loading resource table  'config.hi.apk'
I:    Loading resource table  'config.ja.apk'
I:    Loading resource table  'config.en.apk'
I:    Loading resource table  'config.zh.apk'
I:    Loading resource table  'config.ru.apk'
I:    Loading resource table  'config.es.apk'
I:    Loading resource table  'config.de.apk'
I:    Loading resource table  'config.in.apk'
I:    Loading resource table  'config.ko.apk'
I:    Loading resource table  'config.ar.apk'
I:    Loading resource table  'config.xxxhdpi.apk'
I:    Loading resource table  'config.my.apk'
I:    Loading resource table  'config.it.apk'
I:    Loading resource table  'config.pt.apk'
I:    Loading resource table  'config.tr.apk'
I:    Loading resource table  'df_photomovie.apk'
W:       No resource table found in: 'df_photomovie.apk'
        ERROR=Could not load resources.arsc from file: df_photomovie.apk
I:    Loading resource table  'df_fusing.apk'
I:    Loading resource table  'config.id.apk'
W:       No resource table found in: 'config.id.apk'
        ERROR=Could not load resources.arsc from file: config.id.apk
I:    Loading resource table  'config.fr.apk'
I:    Loading resource table  'config.vi.apk'
I: Decoding AndroidManifest.xml with resources...
I: Loading framework resource table from file: /home/d/apktool/framework/1.apk
I: Regular manifest package...
I: Decoding resources ...
I:        Decoding file-resources packages count=1 ....
I:         [com.ss.android.ugc.trill] 1/1  Decoding file-resources ....
I:                1/9635 current='[base.apk    ]    res/o/a3u.webp'   ->   'drawable-xxhdpi/drawable_0a99'
I:               44/9635 current='[config.xxxhd]      res/p/t.webp'   ->   'drawable-xxxhdpi/drawable_0050'
I:             1093/9635 current='[base.apk    ]      res/j/a2.xml'   ->   'drawable/drawable_004c'
I:             3241/9635 current='[base.apk    ]     res/o/sr.webp'   ->   'drawable-xxhdpi/drawable_07ec'
I:             5662/9635 current='[base.apk    ]    res/a8/aw1.xml'   ->   'layout/layout_09e1'
I:             8161/9635 current='[base.apk    ]    res/a8/are.xml'   ->   'layout/layout_0922'
I:             9635/9635 current='[base.apk    ]    res/o/a0o.webp'   ->   'drawable-xxhdpi/drawable_09df'
I: Decoding values */* XMLs...
I:     Decoding 128  values 
I:    [base.apk] Baksmaling 'classes.dex'  ->  'smali'
I:    [base.apk] Baksmaling 'classes10.dex'  ->  'smali_classes10'
I:    [base.apk] Baksmaling 'classes2.dex'  ->  'smali_classes2'
I:    [base.apk] Baksmaling 'classes3.dex'  ->  'smali_classes3'
I:    [base.apk] Baksmaling 'classes4.dex'  ->  'smali_classes4'
I:    [base.apk] Baksmaling 'classes5.dex'  ->  'smali_classes5'
I:    [base.apk] Baksmaling 'classes6.dex'  ->  'smali_classes6'
I:    [base.apk] Baksmaling 'classes7.dex'  ->  'smali_classes7'
I:    [base.apk] Baksmaling 'classes8.dex'  ->  'smali_classes8'
I:    [base.apk] Baksmaling 'classes9.dex'  ->  'smali_classes9'
I:    [df_photomovie.apk] Baksmaling 'classes.dex'  ->  'smali_classes11'
I:    [df_fusing.apk] Baksmaling 'classes.dex'  ->  'smali_classes12'
I: Copying assets and libs 'base.apk'
I: Copying assets and libs 'config.th.apk'
I: Copying assets and libs 'config.arm64_v8a.apk'
I: Copying assets and libs 'config.hi.apk'
I: Copying assets and libs 'config.ja.apk'
I: Copying assets and libs 'config.en.apk'
I: Copying assets and libs 'config.zh.apk'
I: Copying assets and libs 'config.ru.apk'
I: Copying assets and libs 'config.es.apk'
I: Copying assets and libs 'config.de.apk'
I: Copying assets and libs 'config.in.apk'
I: Copying assets and libs 'config.ko.apk'
I: Copying assets and libs 'config.ar.apk'
I: Copying assets and libs 'config.xxxhdpi.apk'
I: Copying assets and libs 'config.my.apk'
I: Copying assets and libs 'config.it.apk'
I: Copying assets and libs 'config.pt.apk'
I: Copying assets and libs 'config.tr.apk'
I: Copying assets and libs 'df_photomovie.apk'
I: Copying assets and libs 'df_fusing.apk'
I: Copying assets and libs 'config.id.apk'
I: Copying assets and libs 'config.fr.apk'
I: Copying assets and libs 'config.vi.apk'
I: Copying unknown files 'base.apk'
I: Copying unknown files 'config.th.apk'
I: Copying unknown files 'config.arm64_v8a.apk'
I: Copying unknown files 'config.hi.apk'
I: Copying unknown files 'config.ja.apk'
I: Copying unknown files 'config.en.apk'
I: Copying unknown files 'config.zh.apk'
I: Copying unknown files 'config.ru.apk'
I: Copying unknown files 'config.es.apk'
I: Copying unknown files 'config.de.apk'
I: Copying unknown files 'config.in.apk'
I: Copying unknown files 'config.ko.apk'
I: Copying unknown files 'config.ar.apk'
I: Copying unknown files 'config.xxxhdpi.apk'
I: Copying unknown files 'config.my.apk'
I: Copying unknown files 'config.it.apk'
I: Copying unknown files 'config.pt.apk'
I: Copying unknown files 'config.tr.apk'
I: Copying unknown files 'df_photomovie.apk'
I: Copying unknown files 'df_fusing.apk'
I: Copying unknown files 'config.id.apk'
I: Copying unknown files 'config.fr.apk'
I: Copying unknown files 'config.vi.apk'
I: [base.apk] Copying original files...
I: Copying META-INF/services 'base.apk'


```

## Support
* If you like this project, please consider donationation in bitcoin
 ## 1FfTD5pgib7eRJAfNSa3JVTRwoBELBNPRV
 
## Contact
 * thekikfox@gmail.com
