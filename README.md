# **Cài đặt 8 Slots L4D2**

## File Điều Kiện Phải Có:
* [Sourcemod 1.11](https://www.sourcemod.net/downloads.php?branch=stable)
* [Metamod 1.11](https://www.metamodsource.net/downloads.php?branch=stable)
* [Extension-l4dtoolz](https://github.com/Accelerator74/l4dtoolz/releases) By Accelerator74.

## Tùy chọn có thể cài hoặc không cần:

* [Stripper:Source](https://www.bailopan.net/stripper/snapshots/1.2/) 
* [L4D 1/2 Multi-Colors](https://github.com/fbef0102/L4D1_2-Plugins/releases/download/Multi-Colors/multicolors.zip)
* [L4D 1/2 Colors](https://drive.google.com/file/d/1lHjhDIbWa6heb4j7aCPoc6r--FOiEwuT/view?usp=sharing)
* [L4D2 Tickrate Enabler](https://github.com/accelerator74/Tickrate-Enabler/releases/download/build/Tickrate-Enabler-l4d2-def3795.zip)
	- Bỏ **Tickrate_Fixes** nếu bạn sử dụng **Tickrate_Enable**.
- - - -
## Plugin mở rộng - cài đặt - sửa lỗi
* [Left 4 DHooks Direct](https://forums.alliedmods.net/showthread.php?t=321696)
* [Extension-SourceScramble](https://github.com/nosoop/SMExt-SourceScramble/releases/download/0.7.1.1/package.zip)

> Chọn 1 trong các plugin sau để add bot và điều chỉnh survivor:
* [MultiSlots Improved](https://github.com/fbef0102/L4D1_2-Plugins/tree/master/l4dmultislots) By Harry Potter.
     - Plugin 8 slots được nhiều người tin dùng hiện nay, được cập nhật liên tục
     - Chức năng add bot và kiểm soát trang bị người chơi 5+. Chú ý tải thêm phần Require.

* [ABM Alternative](https://forums.alliedmods.net/showpost.php?p=2748953&postcount=517) By Shadowysn.
     - Đây là plugin tôi đang sử dụng và cũng khá ổn định.
     - Với chức năng không kém cạnh Multislots, thêm vào đó là kiểm soát và tính toán cân bằng giữa SI và Survivor.

* [L4D2 Superversus](https://forums.alliedmods.net/showpost.php?p=2704058&postcount=1285) By Shao.
     - Plugin tuy rằng đã lỗi thời nhưng vẫn có một vài server vẫn sử dụng
     - Chức năng siêu mở rộng mà bạn có thể tùy chỉnh số lượng đám common zombie nhỏ số lượng SI spawn và thời gian.
     - Do không có người update. Cũng không biết có hoạt động được nữa hay không.
	
* [Left-4-fix](https://github.com/LuxLuma/Left-4-fix): Sửa lỗi lặt vặt.

* [Survivor Identity Fix for 5+ Survivors (Shadowysn Version)](https://forums.alliedmods.net/showpost.php?p=2718792&postcount=36)
* * Lựa chọn khác [[L4D2]Character_manager (LuxLuma Version)](https://forums.alliedmods.net/showthread.php?t=309601)

* [l4dafkfix_deadbot](https://forums.alliedmods.net/showpost.php?p=2772050&postcount=54): Sửa lỗi khi bạn IDLE mà Bot chết. Bị nhảy sang spec.

* [8+ survivors in rescue vehicle](https://forums.alliedmods.net/showpost.php?p=2771588&postcount=53): Sửa lỗi khi đủ 8 người rescure mới xuất phát.

* [Save Weapon Improved (Harry Version)](https://forums.alliedmods.net/showpost.php?p=2757629&postcount=113):Sửa lỗi mất vũ khí khi qua màn
* * Lựa chọn khác [[L4D2] Transition Restore Fix](https://forums.alliedmods.net/showthread.php?t=336287)

* [Survivor Set Flow Fix](https://forums.alliedmods.net/showthread.php?t=339155): Sửa lỗi map khi bạn ấn gọi rescure nhưng không hoạt động.
* [[L4D/L4D2] Survivor Character Fixes ](https://forums.alliedmods.net/showthread.php?t=336328):Sửa lỗi nội bộ với Survivor Character
* [[L4D & L4D2] Mission and Weapons - Info Editor ](https://forums.alliedmods.net/showthread.php?t=310586)
* [[L4D & L4D2] Use Priority Patch ](https://forums.alliedmods.net/showthread.php?t=327511)

* Copy những cvar dưới đây vào 
    - left4dead2/cfg/listenserver.cfg (nếu không có hãy tụ tạo file)
    - left4dead2/cfg/sourcemod/sourcemod.cfg (nếu không có hãy tụ tạo file)
    ```php
    sv_maxplayers 8 // số người chơi tối đa trong server của bạn
    sv_visiblemaxplayers 8 // cài cho trùng số với số bên trên
    sv_force_unreserved 1 // cho phép người chơi kết nối bằng console
    sv_allow_lobby_connect_only 0 // 1=Chỉ kết nối ở phòng chờ 0=Kết nối ở phòng chờ và giữa game.
    sm_cvar precache_all_survivors 1 // Tải trước các model survivor để tránh crash
    sm_cvar sv_consistency 0 // sử dụng để người khác đỡ bị crash do bạn mod súng (1: Enable, 0: Disable) 
    ```
   - Bạn có thể tham khảo file listenserver.cfg của tôi nếu không biết setup Tickrate: [listenserver.cfg](https://github.com/Kuroneko15/My_server_setup/blob/main/listenserver.cfg)
* 8 Slots Lobby Mod: https://steamcommunity.com/sharedfiles/filedetails/?id=546656726&searchtext=8+slots+lobby
    - Lựa chọn khác nếu muốn bắt đầu chỉ với 1 mình bạn: https://steamcommunity.com/sharedfiles/filedetails/?id=2754956355&searchtext=8+slots+lobby
