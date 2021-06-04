# get_snapshot_from_webcam
upload cam_snapshot_v3.exe, it work for me, and not well tested

如果你有camera接電腦，可以使用這個exe，按Button擷取螢幕快照，儲存到桌面，
如果有多台camera，有列出camera id，可以選擇id切換攝像機


只有一台camera，沒測試過兩台互切，理論上可以


筆電記得要打開"Allow desktop apps to access your camera"，否則會被擋:

左下角Start Button ----> Settings ----> Privacy ---->Camera ----> turn on "Let apps use my camera"


total file size about 50MB

v3.1:
  fix problem: 
  - pyinstaller didn't pack bitmap file(.ico), so I take out the icon file for now
  - every user's desktop path might be different, so I change to use "os.environ['USERPROFILE'])" to adjust it.
  
  work both in my computer and notebook. both are English-language windows.

