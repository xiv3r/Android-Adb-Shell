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
adb shell settings put system min_refresh_rate 0
adb shell settings put system peak_refresh_rate 0
adb shell setprop debug.enable-vr-mode 1
adb shell setprop debug.force-opengl 1
adb shell setprop debug.hwc.force_gpu_vsync 1
adb shell setprop debug.performance.profile 1
adb shell setprop debug.refresh_rate.min_fps 0
adb shell cmd power set-fixed-performance-mode-enabled true
adb shell settings put global window_animation_scale 0
adb shell settings put global transition_animation_scale 0
adb shell settings put global animator_duration_scale 1
adb shell settings put global cached_apps_freezer 1 default 
adb shell settings put global ram_expand_size 2 default 
adb shell settings put global zram 1 default  
adb shell settings put global private_dns_specifier dns.adguard-dns.com 
adb shell settings put secure refresh_rate_mode 2
adb shell set max refresh rate 0 global default
adb shell set min refresh rate 0 global default
adb shell pm trim-caches 128G
adb shell settings put system tube_amp_effect 1 
adb shell settings put system k2hd_effect 1 
adb shell settings put system sound_effects_enabled 0 
adb shell settings put global apply_ramping_ringer 1 
adb shell settings put secure show_notification_snooze 1 
adb shell settings put global restricted_device_performance 0,0 
adb shell settings put global default online_manual_url 0 
adb shell settings put global adaptive_battery_management_enabled 1 
adb shell settings put system intelligent_sleep_mode 1 
adb shell settings put secure adaptive_sleep 1
adb shell settings put secure game_auto_tempature 0
adb shell settings put system rakuten_denwa 0
adb shell settings put system send_security_reports 0
adb shell settings put global sem_enhanced_cpu_responsiveness 1
adb shell settings put global enhanced_processing 2
adb shell settings put system multicore_packet_scheduler 1
adb shell settings put global app_standby_enabled 1
adb shell settings put global cached_apps_freezer enabled
adb shell settings put system mcf_continuity 0
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

