# Android Adb Shell


#### Download: [Ashell](https://github.com/xiv3r/Android-Adb-Shell/raw/main/ashell-v8.apk) | [Shizuku](https://github.com/xiv3r/Android-Adb-Shell/raw/main/shizuku-v13.apk)


## Install



  <p>
    <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/IMG_20231114_092952.jpg"
        </p>
<br></br>
  
<p> 
  <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/IMG_20231114_093015.jpg"
    
  </p>

<br></br>

<p>
  <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/IMG_20231114_093036.jpg" </p>
    
<br></br>

<p>
  <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/Screenshot_2023_1114_092658.png" </p>
    
<br></br>

<p>
  <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/Screenshot_2023_1114_092714.png" </p>
    
<br></br>

<p>
  <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/IMG_20231114_093111.jpg" </p>
    

<br></br>

<p>
  <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/Screenshot_2023_1114_093227.png" </p>
    
<br></br>

<p>
  <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/IMG_20231114_100847.jpg" </p>
    
<br></br>

## Open Ashell Terminal

<p>
  <img align="center" width="500" height="500" src="https://github.com/xiv3r/Android-Adb-Shell/blob/main/file/IMG_20231114_093309.jpg" </p>

# Android Optimization Tweaks

```
adb shell cmd power set-fixed-performance-mode-enabled true
adb shell settings put global cached_apps_freezer 1 default 
adb shell settings put global ram_expand_size 0 default 
adb shell settings put global zram 1 default 
adb shell settings put global default windows_antimation_scale 0.0
adb shell settings put global default transition_animation_scale 0.0
adb shell settings put global default animator_duration_scale 0.0
adb shell settings put system peak_refresh_rate 120.0 
adb shell settings put system min_refresh_rate 120.0 
adb shell settings put global default private_dns_specifier dns.adguard-dns.com 
adb shell settings put system default multicore_packet_scheduler 1 
adb shell settings put secure default refresh_rate_mode 2
adb shell set max refresh rate 120 global default 
adb shell set min refresh rate 120 global default 
adb shell pm trim-caches 128G
adb shell settings put system default tube_amp_effect 1 
adb shell settings put system default k2hd_effect 1 
adb shell settings put system default sound_effects_enabled 0 
adb shell settings put global default apply_ramping_ringer 1 
adb shell settings put secure default show_notification_snooze 1 
adb shell settings put system default rakuten_denwa 0 
adb shell settings put system default send_security_reports 0 
adb shell settings put global default sem_enhanced_cpu_responsiveness 1 
adb shell settings put global default restricted_device_performance 0,0 
adb shell settings put global default online_manual_url 0 
adb shell settings put global default adaptive_battery_management_enabled 1 
adb shell settings put system default intelligent_sleep_mode 1 
adb shell settings put secure default adaptive_sleep 1
adb shell settings put secure default game_auto_tempature 0
adb shell settings put system default rakuten_denwa 0
adb shell settings put system default send_security_reports 0
adb shell settings put global default sem_enhanced_cpu_responsiveness 1
adb shell settings put global default enhanced_processing 2
adb shell settings put system default multicore_packet_scheduler 1
adb shell settings put global default app_standby_enabled 1
adb shell settings put global default cached_apps_freezer enabled
adb shell settings put system default mcf_continuity 0
```

# This commands will disable the phantom process killer:

```
adb shell /system/bin/device_config set_sync_disabled_for_tests persistent

adb shell /system/bin/device_config put activity_manager max_phantom_processes 2147483647

adb shell settings put global settings_enable_monitor_phantom_procs false
```

To verify:

```
adb shell /system/bin/dumpsys activity settings | grep max_phantom_processes

adb shell /system/bin/device_config get activity_manager max_phantom_processes
```

