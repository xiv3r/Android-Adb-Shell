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

- adb shell settings list global > global_stock.txt
- adb shell settings list system > system_stock.txt
- adb shell settings list secure > secure_stock.txt
If you want to check a parameter's value, replace "put" with "get" and remove value.
Ex: adb shell settings get global animator_duration_scale

Improve Display Performance 
- adb shell settings put system screen_brightness_mode 1
- adb shell settings put system screen_auto_brightness_adj 0.9
- adb shell settings put global burn_in_protection 1
- adb shell settings put system peak_refresh_rate 120.0 #Sets max refresh rate to 120
- adb shell settings put system min_refresh_rate 1.0 #Sets min refresh rate to 1
- adb shell settings put system display_color_mode 3
- adb shell settings put global window_animation_scale 0.4
- adb shell settings put global transition_animation_scale 0.4
- adb shell settings put global animator_duration_scale 0.4
Enable New Back Gesture Animation 
- adb shell settings put global enable_back_animation 1
Improve Power Management 
- adb shell settings put global cached_apps_freezer enabled
- adb shell settings put global adaptive_battery_management_enabled 0
- adb shell settings put global app_restriction_enabled true
- adb shell settings put global app_standby_enabled 1
- adb shell settings put secure adaptive_charging_enabled 0
- adb shell settings put secure adaptive_connectivity_enabled 0
- adb shell settings put secure adaptive_sleep 0
- adb shell settings put global automatic_power_save_mode 0
- adb shell settings put global dynamic_power_savings_disable_threshold 20
- adb shell settings put global dynamic_power_savings_enabled 0
- adb shell settings put global low_power 0
Disable Google Stuff 
- adb shell settings put secure smartspace 0
- adb shell settings put secure systemui.google.opa_enabled 0
- adb shell settings put system system gearhead:driving_mode_settings_enabled 0
- adb shell settings put global hotword_detection_enabled 0
Improve System Performance 
- adb shell settings put global zram_enabled 0
- adb shell settings put global disable_window_blurs 1
Improve Networking Performance 
- adb shell settings put global network_recommendations_enabled 0
- adb shell settings put global network_scoring_ui_enabled 0
- adb shell settings put global tether_offload_disabled 0
- adb shell settings put global wifi_power_save 0
- adb shell settings put global wifi_scan_always_enabled 0
- adb shell settings put global enable_cellular_on_boot 1
- adb shell settings put global mobile_data_always_on 0
- adb shell settings put global ble_scan_always_enabled 0
- adb shell settings put global assisted_gps_enabled 1
Disable Gestures 
- adb shell settings put global ambient_enabled 0
- adb shell settings put global ambient_tilt_to_wake 0
- adb shell settings put global ambient_touch_to_wake 0
- adb shell settings put secure aware_enabled 0
- adb shell settings put secure doze_enabled 0
- adb shell settings put secure doze_always_on 0
- adb shell settings put secure doze_tap_gesture 0
- adb shell settings put secure doze_on_pick_up 0
- adb shell settings put secure doze_on_double_tap 0
- adb shell settings put secure camera_double_twist_to_flip_enabled 0
- adb shell settings put secure double_tap_to_sleep 0
- adb shell settings put secure double_tap_to_wake 0
- adb shell settings put secure double_tap_to_wake_up 0
- adb shell settings put system lift_to_wake 0
- adb shell settings put secure hush_gesture_used 0
- adb shell settings put secure volume_hush_gesture 0
- adb shell settings put secure silence_gesture 0
- adb shell settings put secure skip_gesture 0
- adb shell settings put secure wake_gesture_enabled 0
- adb shell settings put secure one_handed_mode_activated 0
- adb shell settings put secure one_handed_mode_enabled 0
Disable Sound & Vibration Feedback 
- adb shell settings put global power_sounds_enabled 0
- adb shell settings put secure charging_sounds_enabled 0
- adb shell settings put system charging_vibration_enabled 1
- adb shell settings put system lockscreen_sounds_enabled 0
- adb shell settings put system sound_effects_enabled 0
- adb shell settings put system dtmf_tone 0
- adb shell settings put system haptic_feedback_enabled 0
- adb shell settings put system haptic_feedback_intensity 0
- adb shell settings put system hardware_haptic_feedback_intensity 0
- adb shell settings put system media_vibration_intensity 0
- adb shell settings put system notification_light_pulse 0
Improve Vibrations 
- adb shell settings put system vibrate_when_ringing 1
- adb shell settings put system ring_vibration_intensity 3
- adb shell settings put system notification_vibration_intensity 3
Disable Screen Saver 
- adb shell settings put secure screensaver_enabled 0
- adb shell settings put secure screensaver_activate_on_sleep 0
- adb shell settings put secure screensaver_activate_on_dock 0
Disable Captions 
- adb shell settings put secure odi_captions_enabled 0
- adb shell settings put secure odi_captions_volume_ui_enabled 0
- adb shell settings put secure accessibility_captioning_enabled 0
- adb shell settings put secure ui_translation_enabled 0
Boost Apps 
- adb shell cmd package compile -m speed-profile -a
Boost Battery 
- adb shell cmd package bg-dexopt-job
Clear All Apps Cache (Enter multiple times) 
- adb shell pm trim-caches 999999999999999999 (Enter multiple times for it to be effective)
Force Stop Apps 
- adb shell am force-stop com.package.name (Create a .bat file containing all packages)
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

