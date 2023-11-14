# Android Adb Shell


#### Download: [Ashell](https://github.com/xiv3r/Android-Adb-Shell/raw/main/ashell-v8.apk) | [Shizuku](https://github.com/xiv3r/Android-Adb-Shell/raw/main/shizuku-v13.apk)


## Install



  <p> <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/IMG_20231114_092952.jpg"
        </p>

  
<p> <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/IMG_20231114_093015.jpg"
    
  </p>

<br>

<p>
  <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/IMG_20231114_093036.jpg" </p>
    
<br>

<p>
  <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/Screenshot_2023_1114_092658.png" </p>
    
<br>

<p>
  <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/Screenshot_2023_1114_092714.png" </p>
    
<br>

<p>
  <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/IMG_20231114_093111.jpg" </p>
    
<br>

<p>
  <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/Screenshot_2023_1114_093227.png" </p>
    
<br>

<p>
  <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/IMG_20231114_100847.jpg" </p>
    
<br>

- Open Ashell Terminal

<p>
  <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/IMG_20231114_093309.jpg" </p>

# Android Optimization Tweaks
```
adb shell cmd power set-fixed-performance-mode-enabled true
adb shell settings put global cached_apps_freezer 1 default 
adb shell settings put global ram_expand_size 0 default 
adb shell settings put global zram 0 default 
adb shell settings put global default windows_antimation_scale 0.25 
adb shell settings put global default transition_animation_scale 0.25 
adb shell settings put global default animator_duration_scale 0.25 
adb shell settings put system peak_refresh_rate 120.0 
adb shell settings put system min_refresh_rate 120.0 
adb shell settings put global private_dns_specifier dns.adguard-dns.com 
adb shell settings put system multicore_packet_scheduler 1 
adb shell settings put secure refresh_rate_mode 2
adb shell set max refresh rate 120 global default 
adb shell set min refresh rate 120 global default 
adb shell pm trim-caches 128G adb shell settings put system tube_amp_effect 1 
adb shell settings put system k2hd_effect 1 
adb shell settings put system sound_effects_enabled 0 
adb shell settings put global apply_ramping_ringer 1 
adb shell settings put secure show_notification_snooze 1 
adb shell settings put system rakuten_denwa 0 
adb shell settings put system send_security_reports 0 
adb shell settings put global sem_enhanced_cpu_responsiveness 1 
adb shell settings put global restricted_device_performance 0,0 
adb shell settings put global online_manual_url 0 
adb shell settings put global adaptive_battery_management_enabled 1 
adb shell settings put system intelligent_sleep_mode 1 
adb shell settings put secure adaptive_sleep 1
```
