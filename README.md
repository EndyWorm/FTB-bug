# FTB-bug
LOG
Process:               launcher [6808]
Path:                  /Users/USER/Library/Application Support/.ftba/*/Minecraft.app/Contents/MacOS/launcher
Identifier:            com.mojang.minecraftlauncher
Version:               883 (1)
Code Type:             X86-64 (Native)
Parent Process:        ??? [1]
Responsible:           launcher [6808]
User ID:               501

Date/Time:             2021-02-19 11:06:24.828 +0100
OS Version:            Mac OS X 10.15.7 (19H114)
Report Version:        12
Bridge OS Version:     5.1 (18P3030)
Anonymous UUID:        BBBD84EB-CC6C-3865-0C3E-C0C66752A74C

Sleep/Wake UUID:       199441C3-1E12-4631-BB3C-9002818C2590

Time Awake Since Boot: 29000 seconds
Time Since Wake:       8000 seconds

System Integrity Protection: enabled

Crashed Thread:        0  Dispatch queue: com.apple.main-thread

Exception Type:        EXC_CRASH (SIGABRT)
Exception Codes:       0x0000000000000000, 0x0000000000000000
Exception Note:        EXC_CORPSE_NOTIFY

Application Specific Information:
abort() called
terminating with uncaught exception of type std::runtime_error: collate_byname<char>::collate_byname failed to construct for 

Thread 0 Crashed:: Dispatch queue: com.apple.main-thread
0   libsystem_kernel.dylib        	0x00007fff7283e33a __pthread_kill + 10
1   libsystem_pthread.dylib       	0x00007fff728fae60 pthread_kill + 430
2   libsystem_c.dylib             	0x00007fff727c5808 abort + 120
3   libc++abi.dylib               	0x00007fff6fa26458 abort_message + 231
4   libc++abi.dylib               	0x00007fff6fa178a7 demangling_terminate_handler() + 238
5   libobjc.A.dylib               	0x00007fff715505b1 _objc_terminate() + 104
6   libc++abi.dylib               	0x00007fff6fa25887 std::__terminate(void (*)()) + 8
7   libc++abi.dylib               	0x00007fff6fa28387 __cxa_rethrow + 99
8   libc++.1.dylib                	0x00007fff6f9ea5c3 std::__1::locale::__imp::__imp(std::__1::basic_string<char, std::__1::char_traits<char>, std::__1::allocator<char> > const&, unsigned long) + 1531
9   libc++.1.dylib                	0x00007fff6f9ebb21 std::__1::locale::locale(char const*) + 63
10  com.mojang.minecraftlauncher  	0x000000010f48fce2 util::toLower(std::__1::basic_string_view<char, std::__1::char_traits<char> >) (.cold.1) + 34
11  com.mojang.minecraftlauncher  	0x000000010f40581b util::toLower(std::__1::basic_string_view<char, std::__1::char_traits<char> >) + 347
12  com.mojang.minecraftlauncher  	0x000000010f3add02 (anonymous namespace)::startsWithCaseInsensitive(std::__1::basic_string<char, std::__1::char_traits<char>, std::__1::allocator<char> > const&, std::__1::basic_string<char, std::__1::char_traits<char>, std::__1::allocator<char> > const&) + 50
13  com.mojang.minecraftlauncher  	0x000000010f3aa784 Settings::Settings(std::__1::vector<std::__1::basic_string<char, std::__1::char_traits<char>, std::__1::allocator<char> >, std::__1::allocator<std::__1::basic_string<char, std::__1::char_traits<char>, std::__1::allocator<char> > > >&) + 1108
14  com.mojang.minecraftlauncher  	0x000000010f37f246 commonSetup(std::__1::vector<std::__1::basic_string<char, std::__1::char_traits<char>, std::__1::allocator<char> >, std::__1::allocator<std::__1::basic_string<char, std::__1::char_traits<char>, std::__1::allocator<char> > > >&) + 38
15  com.mojang.minecraftlauncher  	0x000000010f387885 main + 1653
16  libdyld.dylib                 	0x00007fff726f6cc9 start + 1

Thread 0 crashed with X86 Thread State (64-bit):
  rax: 0x0000000000000000  rbx: 0x0000000118437dc0  rcx: 0x00007ffee0884458  rdx: 0x0000000000000000
  rdi: 0x0000000000000307  rsi: 0x0000000000000006  rbp: 0x00007ffee0884480  rsp: 0x00007ffee0884458
   r8: 0x00007ffee0884320   r9: 0x00007ffee08844f0  r10: 0x0000000118437dc0  r11: 0x0000000000000246
  r12: 0x0000000000000307  r13: 0x0000003000000008  r14: 0x0000000000000006  r15: 0x0000000000000016
  rip: 0x00007fff7283e33a  rfl: 0x0000000000000246  cr2: 0x000000010f49454c
  
Logical CPU:     0
Error Code:      0x02000148
Trap Number:     133


Binary Images:
       0x10f37a000 -        0x10f4f1fff +com.mojang.minecraftlauncher (883 - 1) <08AD25E7-D85A-3179-8646-CD574AACF575> /Users/USER/Library/Application Support/.ftba/*/Minecraft.app/Contents/MacOS/launcher
       0x11836d000 -        0x1183fef47  dyld (750.6) <F58DDECD-315C-3B7C-8162-A5E8E1D62FE3> /usr/lib/dyld
    0x7fff34291000 -     0x7fff34291fff  com.apple.Accelerate (1.11 - Accelerate 1.11) <4F9977AE-DBDB-3A16-A536-AC1F9938DCDD> /System/Library/Frameworks/Accelerate.framework/Versions/A/Accelerate
    0x7fff342a9000 -     0x7fff348fffff  com.apple.vImage (8.1 - 524.2.1) <EA6F5FF2-7A1B-35D5-A5A3-D2B3386ECB75> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vImage.framework/Versions/A/vImage
    0x7fff34900000 -     0x7fff34b67ff7  libBLAS.dylib (1303.60.1) <C6C2D42F-7456-3DBF-8BE2-9AA06EFC78FD> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libBLAS.dylib
    0x7fff34b68000 -     0x7fff3503bfef  libBNNS.dylib (144.100.2) <99C61C48-B14C-3DA6-8C31-6BF72DA0A3A9> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libBNNS.dylib
    0x7fff3503c000 -     0x7fff353d7fff  libLAPACK.dylib (1303.60.1) <5E3E3867-50C3-3E6A-9A2E-007CE77A4641> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libLAPACK.dylib
    0x7fff353d8000 -     0x7fff353edfec  libLinearAlgebra.dylib (1303.60.1) <3D433800-0099-33E0-8C81-15F83247B2C9> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libLinearAlgebra.dylib
    0x7fff353ee000 -     0x7fff353f3ff3  libQuadrature.dylib (7) <371F36A7-B12F-363E-8955-F24F7C2048F6> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libQuadrature.dylib
    0x7fff353f4000 -     0x7fff35464fff  libSparse.dylib (103) <B8A10D0C-4577-343D-B310-A3E81265D107> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libSparse.dylib
    0x7fff35465000 -     0x7fff35477fef  libSparseBLAS.dylib (1303.60.1) <B147FEF6-A0DB-3830-BF06-45BEC58DB576> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libSparseBLAS.dylib
    0x7fff35478000 -     0x7fff3564ffd7  libvDSP.dylib (735.140.1) <D63DC0A5-B8B4-3562-A574-E73BC3B57407> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libvDSP.dylib
    0x7fff35650000 -     0x7fff35712fef  libvMisc.dylib (735.140.1) <3601FDE3-B142-398D-987D-8151A51F0A96> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libvMisc.dylib
    0x7fff35713000 -     0x7fff35713fff  com.apple.Accelerate.vecLib (3.11 - vecLib 3.11) <F6C5613D-2284-342B-9160-9731F78B4DE5> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/vecLib
    0x7fff358bd000 -     0x7fff3667dff2  com.apple.AppKit (6.9 - 1894.60.100) <322D043D-1140-3486-9523-3F56FF4D8349> /System/Library/Frameworks/AppKit.framework/Versions/C/AppKit
    0x7fff366cd000 -     0x7fff366cdfff  com.apple.ApplicationServices (48 - 50) <20CF59CD-A395-3570-A4DB-589D55C70B3F> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/ApplicationServices
    0x7fff366ce000 -     0x7fff36739fff  com.apple.ApplicationServices.ATS (377 - 493.0.4.1) <87EA5DE1-506A-39FD-88BE-D8A3416C9012> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/ATS.framework/Versions/A/ATS
    0x7fff367d2000 -     0x7fff36810ff0  libFontRegistry.dylib (274.0.5.1) <F3461C05-0370-359B-9F03-5C1C1F7763EC> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/ATS.framework/Versions/A/Resources/libFontRegistry.dylib
    0x7fff3686b000 -     0x7fff3689afff  com.apple.ATSUI (1.0 - 1) <5F513967-DDD7-3F22-AD14-8A38ABD9F2D0> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/ATSUI.framework/Versions/A/ATSUI
    0x7fff3689b000 -     0x7fff3689fffb  com.apple.ColorSyncLegacy (4.13.0 - 1) <72EE68DB-F069-37F5-AA2A-40D5FCF139F4> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/ColorSyncLegacy.framework/Versions/A/ColorSyncLegacy
    0x7fff36939000 -     0x7fff36990ffa  com.apple.HIServices (1.22 - 676) <14DF4D42-E24D-3EBD-9A9D-93124D8D6AA1> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/HIServices.framework/Versions/A/HIServices
    0x7fff36991000 -     0x7fff3699ffff  com.apple.LangAnalysis (1.7.0 - 1.7.0) <01B8B6B3-E2C3-3607-B34A-8283A7E0E924> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/LangAnalysis.framework/Versions/A/LangAnalysis
    0x7fff369a0000 -     0x7fff369e5ffa  com.apple.print.framework.PrintCore (15.4 - 516.2) <437BCF12-48D2-3770-8BC9-567718FB1BCA> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/PrintCore.framework/Versions/A/PrintCore
    0x7fff369e6000 -     0x7fff369f0ff7  com.apple.QD (4.0 - 413) <27A36D07-B5E9-32E6-87B6-3127F260F48D> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/QD.framework/Versions/A/QD
    0x7fff369f1000 -     0x7fff369feffc  com.apple.speech.synthesis.framework (9.0.24 - 9.0.24) <75344F8F-32CA-3558-B4E6-F56D498250E4> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/SpeechSynthesis.framework/Versions/A/SpeechSynthesis
    0x7fff369ff000 -     0x7fff36ae0ffa  com.apple.audio.toolbox.AudioToolbox (1.14 - 1.14) <6185BF20-D2E7-3812-8FD8-EC5237672104> /System/Library/Frameworks/AudioToolbox.framework/Versions/A/AudioToolbox
    0x7fff36ae2000 -     0x7fff36ae2fff  com.apple.audio.units.AudioUnit (1.14 - 1.14) <918ED3EB-0232-31F3-9BF5-18D1CB11523F> /System/Library/Frameworks/AudioUnit.framework/Versions/A/AudioUnit
    0x7fff36e79000 -     0x7fff37208ffa  com.apple.CFNetwork (1128.0.1 - 1128.0.1) <07F9CA9C-B954-3EA0-A710-3122BFF9F057> /System/Library/Frameworks/CFNetwork.framework/Versions/A/CFNetwork
    0x7fff37289000 -     0x7fff3757dff3  com.apple.HIToolbox (2.1.1 - 994.6) <EAF2DAC3-66B1-30BF-AF10-72DDA90D1044> /System/Library/Frameworks/Carbon.framework/Versions/A/Frameworks/HIToolbox.framework/Versions/A/HIToolbox
    0x7fff375c8000 -     0x7fff375cefff  com.apple.speech.recognition.framework (6.0.3 - 6.0.3) <9614A01E-8303-3422-A3BA-6CE27540E09A> /System/Library/Frameworks/Carbon.framework/Versions/A/Frameworks/SpeechRecognition.framework/Versions/A/SpeechRecognition
    0x7fff37768000 -     0x7fff37768fff  com.apple.Cocoa (6.11 - 23) <85C8B9B4-6F0B-3BD5-8934-C299FE481A44> /System/Library/Frameworks/Cocoa.framework/Versions/A/Cocoa
    0x7fff37776000 -     0x7fff3786cfff  com.apple.ColorSync (4.13.0 - 3394.9) <A126406C-DA38-3FFE-8B25-BB9859EFD159> /System/Library/Frameworks/ColorSync.framework/Versions/A/ColorSync
    0x7fff37b57000 -     0x7fff38060ffb  com.apple.audio.CoreAudio (5.0 - 5.0) <47923B12-3D14-328A-9C86-27A3A2A73068> /System/Library/Frameworks/CoreAudio.framework/Versions/A/CoreAudio
    0x7fff380b3000 -     0x7fff380ebfff  com.apple.CoreBluetooth (1.0 - 1) <23DBB313-A082-3C08-8E1F-2D31EE4247EF> /System/Library/Frameworks/CoreBluetooth.framework/Versions/A/CoreBluetooth
    0x7fff380ec000 -     0x7fff384d6fe8  com.apple.CoreData (120 - 977.3) <49AE61CA-C91E-31FE-9BD0-1AACFFB5181E> /System/Library/Frameworks/CoreData.framework/Versions/A/CoreData
    0x7fff384d7000 -     0x7fff38609ff6  com.apple.CoreDisplay (1.0 - 186.6.15) <213D7011-8180-3CF4-9BE7-FB8F75DCDB95> /System/Library/Frameworks/CoreDisplay.framework/Versions/A/CoreDisplay
    0x7fff3860a000 -     0x7fff38a89feb  com.apple.CoreFoundation (6.9 - 1677.201) <56B0FE5F-D493-3DF1-ABFF-ECC450268B97> /System/Library/Frameworks/CoreFoundation.framework/Versions/A/CoreFoundation
    0x7fff38a8b000 -     0x7fff39100ff8  com.apple.CoreGraphics (2.0 - 1355.22) <4A3CDE7B-4578-3058-966A-3D1DC095A935> /System/Library/Frameworks/CoreGraphics.framework/Versions/A/CoreGraphics
    0x7fff3910e000 -     0x7fff39469ff0  com.apple.CoreImage (15.0.0 - 940.9) <69361069-01AB-342E-862B-73A74271A765> /System/Library/Frameworks/CoreImage.framework/Versions/A/CoreImage
    0x7fff399f2000 -     0x7fff399f2fff  com.apple.CoreServices (1069.24 - 1069.24) <2D1A6C60-DD34-368F-88FF-E39C9FE549A9> /System/Library/Frameworks/CoreServices.framework/Versions/A/CoreServices
    0x7fff399f3000 -     0x7fff39a78fff  com.apple.AE (838.1 - 838.1) <2E5FD5AE-8A7F-353F-9BD1-0241F3586181> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/AE.framework/Versions/A/AE
    0x7fff39a79000 -     0x7fff39d5aff7  com.apple.CoreServices.CarbonCore (1217 - 1217) <BE379206-99FA-30CD-8391-2708473A633F> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/CarbonCore.framework/Versions/A/CarbonCore
    0x7fff39d5b000 -     0x7fff39da8ffd  com.apple.DictionaryServices (1.2 - 323.6) <26B70C82-25BC-353A-858F-945B14C803A2> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/DictionaryServices.framework/Versions/A/DictionaryServices
    0x7fff39da9000 -     0x7fff39db1ff7  com.apple.CoreServices.FSEvents (1268.100.1 - 1268.100.1) <FC84DB48-A3CE-30F7-A918-B3587731ACC7> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/FSEvents.framework/Versions/A/FSEvents
    0x7fff39db2000 -     0x7fff39fecff6  com.apple.LaunchServices (1069.24 - 1069.24) <9A5359D9-9148-3B18-B868-56A9DA5FB60C> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/LaunchServices.framework/Versions/A/LaunchServices
    0x7fff39fed000 -     0x7fff3a085ff1  com.apple.Metadata (10.7.0 - 2076.7) <0973F7E5-D58C-3574-A3CE-4F12CAC2D4C7> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/Metadata.framework/Versions/A/Metadata
    0x7fff3a086000 -     0x7fff3a0b3fff  com.apple.CoreServices.OSServices (1069.24 - 1069.24) <0E4F48AD-402C-3E9D-9CA9-6DD9479B28F9> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/OSServices.framework/Versions/A/OSServices
    0x7fff3a0b4000 -     0x7fff3a11bfff  com.apple.SearchKit (1.4.1 - 1.4.1) <2C5E1D85-E8B1-3DC5-91B9-E3EDB48E9369> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/SearchKit.framework/Versions/A/SearchKit
    0x7fff3a11c000 -     0x7fff3a140ff5  com.apple.coreservices.SharedFileList (131.4 - 131.4) <02DE0D56-E371-3EF5-9BC1-FA435451B412> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/SharedFileList.framework/Versions/A/SharedFileList
    0x7fff3a465000 -     0x7fff3a61cffc  com.apple.CoreText (643.1.5.2 - 643.1.5.2) <ADDE38C3-C247-34AD-9903-0276050E242C> /System/Library/Frameworks/CoreText.framework/Versions/A/CoreText
    0x7fff3a61d000 -     0x7fff3a661ffb  com.apple.CoreVideo (1.8 - 344.3) <5314E70D-325F-3E98-99FC-00FDF520747E> /System/Library/Frameworks/CoreVideo.framework/Versions/A/CoreVideo
    0x7fff3a662000 -     0x7fff3a6efffc  com.apple.framework.CoreWLAN (13.0 - 1601.2) <6223BFD5-D451-3DE9-90F6-F609AC0B0027> /System/Library/Frameworks/CoreWLAN.framework/Versions/A/CoreWLAN
    0x7fff3a986000 -     0x7fff3a98cfff  com.apple.DiskArbitration (2.7 - 2.7) <0BBBB6A6-604D-368B-9943-50B8CE75D51D> /System/Library/Frameworks/DiskArbitration.framework/Versions/A/DiskArbitration
    0x7fff3acc7000 -     0x7fff3b08cfff  com.apple.Foundation (6.9 - 1677.201) <E020DC09-4221-3961-A450-638525789B38> /System/Library/Frameworks/Foundation.framework/Versions/C/Foundation
    0x7fff3b0f9000 -     0x7fff3b149ff7  com.apple.GSS (4.0 - 2.0) <2F3A67E6-D42A-3CF0-9041-A42C22D46F95> /System/Library/Frameworks/GSS.framework/Versions/A/GSS
    0x7fff3b286000 -     0x7fff3b39aff3  com.apple.Bluetooth (7.0.6 - 7.0.6f8) <C7AF719C-51B4-3727-A947-EB01204272D9> /System/Library/Frameworks/IOBluetooth.framework/Versions/A/IOBluetooth
    0x7fff3b400000 -     0x7fff3b4a4ff3  com.apple.framework.IOKit (2.0.2 - 1726.140.1) <14223387-6F81-3976-8605-4BC2F253A93E> /System/Library/Frameworks/IOKit.framework/Versions/A/IOKit
    0x7fff3b4a6000 -     0x7fff3b4b7ffb  com.apple.IOSurface (269.11 - 269.11) <BCD744D4-E17E-3C2E-B69C-F69C789892E9> /System/Library/Frameworks/IOSurface.framework/Versions/A/IOSurface
    0x7fff3b536000 -     0x7fff3b693fee  com.apple.ImageIO.framework (3.3.0 - 1976.11.4) <6FC6EE76-F76F-312C-9C67-4B9F0E0B832A> /System/Library/Frameworks/ImageIO.framework/Versions/A/ImageIO
    0x7fff3b694000 -     0x7fff3b697fff  libGIF.dylib (1976.11.4) <F57785E7-6FDA-30A1-B926-CD4D727B56DC> /System/Library/Frameworks/ImageIO.framework/Versions/A/Resources/libGIF.dylib
    0x7fff3b698000 -     0x7fff3b751fe7  libJP2.dylib (1976.11.4) <A6CC541D-37C4-3A90-86B0-2F67B917B4EE> /System/Library/Frameworks/ImageIO.framework/Versions/A/Resources/libJP2.dylib
    0x7fff3b752000 -     0x7fff3b775fe3  libJPEG.dylib (1976.11.4) <37FA33BD-1C78-3FA6-8D35-3F3755462597> /System/Library/Frameworks/ImageIO.framework/Versions/A/Resources/libJPEG.dylib
    0x7fff3b9f2000 -     0x7fff3ba0cfef  libPng.dylib (1976.11.4) <1AD4B940-5B1F-39A4-873C-9C568AA287B7> /System/Library/Frameworks/ImageIO.framework/Versions/A/Resources/libPng.dylib
    0x7fff3ba0d000 -     0x7fff3ba0efff  libRadiance.dylib (1976.11.4) <868D2C2C-1909-31B1-A0C2-C971F0BE1EC5> /System/Library/Frameworks/ImageIO.framework/Versions/A/Resources/libRadiance.dylib
    0x7fff3ba0f000 -     0x7fff3ba55fff  libTIFF.dylib (1976.11.4) <1125DCD0-337D-3E01-84F9-106DEEEA5715> /System/Library/Frameworks/ImageIO.framework/Versions/A/Resources/libTIFF.dylib
    0x7fff3cfb7000 -     0x7fff3cfc9ff3  com.apple.Kerberos (3.0 - 1) <03BB492B-016E-37BF-B020-39C2CF7487FE> /System/Library/Frameworks/Kerberos.framework/Versions/A/Kerberos
    0x7fff3cfca000 -     0x7fff3cfcafff  libHeimdalProxy.dylib (77) <0A2905EE-9533-3345-AF9B-AAC71513BDFD> /System/Library/Frameworks/Kerberos.framework/Versions/A/Libraries/libHeimdalProxy.dylib
    0x7fff3db81000 -     0x7fff3dc4bfff  com.apple.Metal (212.8 - 212.8) <98C944D6-62C8-355E-90F8-C1CA2429EF24> /System/Library/Frameworks/Metal.framework/Versions/A/Metal
    0x7fff3dc68000 -     0x7fff3dca5ff7  com.apple.MetalPerformanceShaders.MPSCore (1.0 - 1) <7EBAC15D-7837-395D-B405-1E29F7DA68FA> /System/Library/Frameworks/MetalPerformanceShaders.framework/Frameworks/MPSCore.framework/Versions/A/MPSCore
    0x7fff3dca6000 -     0x7fff3dd30fe2  com.apple.MetalPerformanceShaders.MPSImage (1.0 - 1) <B424FE0C-6E90-3BFA-A6E7-DD86C735AE90> /System/Library/Frameworks/MetalPerformanceShaders.framework/Frameworks/MPSImage.framework/Versions/A/MPSImage
    0x7fff3dd31000 -     0x7fff3dd56ff4  com.apple.MetalPerformanceShaders.MPSMatrix (1.0 - 1) <02006D92-E2AB-3892-A96B-37F6520C19BA> /System/Library/Frameworks/MetalPerformanceShaders.framework/Frameworks/MPSMatrix.framework/Versions/A/MPSMatrix
    0x7fff3dd57000 -     0x7fff3dd6cffb  com.apple.MetalPerformanceShaders.MPSNDArray (1.0 - 1) <CAA5A368-DB71-34F6-AEF9-27A8BC298F53> /System/Library/Frameworks/MetalPerformanceShaders.framework/Frameworks/MPSNDArray.framework/Versions/A/MPSNDArray
    0x7fff3dd6d000 -     0x7fff3decbffc  com.apple.MetalPerformanceShaders.MPSNeuralNetwork (1.0 - 1) <05612E06-50CB-318F-9F8E-EF4D49FAB3B0> /System/Library/Frameworks/MetalPerformanceShaders.framework/Frameworks/MPSNeuralNetwork.framework/Versions/A/MPSNeuralNetwork
    0x7fff3decc000 -     0x7fff3df1bff4  com.apple.MetalPerformanceShaders.MPSRayIntersector (1.0 - 1) <B0B591F8-6875-351E-867F-8EB3CD38CD52> /System/Library/Frameworks/MetalPerformanceShaders.framework/Frameworks/MPSRayIntersector.framework/Versions/A/MPSRayIntersector
    0x7fff3df1c000 -     0x7fff3df1dff5  com.apple.MetalPerformanceShaders.MetalPerformanceShaders (1.0 - 1) <F2921F9A-3041-3495-878D-64134267B847> /System/Library/Frameworks/MetalPerformanceShaders.framework/Versions/A/MetalPerformanceShaders
    0x7fff3efab000 -     0x7fff3efb7ffe  com.apple.NetFS (6.0 - 4.0) <4415F027-D36D-3B9C-96BA-AD22B44A4722> /System/Library/Frameworks/NetFS.framework/Versions/A/NetFS
    0x7fff3efb8000 -     0x7fff3f10fff3  com.apple.Network (1.0 - 1) <4A0F3B93-4D23-3E74-9A3D-AD19E9C0E59E> /System/Library/Frameworks/Network.framework/Versions/A/Network
    0x7fff41b41000 -     0x7fff41b99fff  com.apple.opencl (3.5 - 3.5) <293FE223-9186-320B-81A4-EC8104C38357> /System/Library/Frameworks/OpenCL.framework/Versions/A/OpenCL
    0x7fff41b9a000 -     0x7fff41bb6fff  com.apple.CFOpenDirectory (10.15 - 220.40.1) <7E6C88EB-3DD9-32B0-81FC-179552834FA9> /System/Library/Frameworks/OpenDirectory.framework/Versions/A/Frameworks/CFOpenDirectory.framework/Versions/A/CFOpenDirectory
    0x7fff41bb7000 -     0x7fff41bc2ffd  com.apple.OpenDirectory (10.15 - 220.40.1) <4A92D8D8-A9E5-3A9C-942F-28576F6BCDF5> /System/Library/Frameworks/OpenDirectory.framework/Versions/A/OpenDirectory
    0x7fff42528000 -     0x7fff4252afff  libCVMSPluginSupport.dylib (17.10.22) <2B6C3C16-3F5F-36A8-8070-2A862B90328B> /System/Library/Frameworks/OpenGL.framework/Versions/A/Libraries/libCVMSPluginSupport.dylib
    0x7fff4252b000 -     0x7fff42530fff  libCoreFSCache.dylib (176.15) <E9A20E72-B17F-33D6-8894-41934A10B822> /System/Library/Frameworks/OpenGL.framework/Versions/A/Libraries/libCoreFSCache.dylib
    0x7fff42531000 -     0x7fff42535fff  libCoreVMClient.dylib (176.15) <018A48BA-1326-3847-8FB5-A7C99322EB87> /System/Library/Frameworks/OpenGL.framework/Versions/A/Libraries/libCoreVMClient.dylib
    0x7fff42536000 -     0x7fff4253eff7  libGFXShared.dylib (17.10.22) <AB47B927-65E3-3924-88BE-0A5BE7906785> /System/Library/Frameworks/OpenGL.framework/Versions/A/Libraries/libGFXShared.dylib
    0x7fff4253f000 -     0x7fff42549fff  libGL.dylib (17.10.22) <FB5E6A75-398E-38EF-8CB2-59F5BFE3034C> /System/Library/Frameworks/OpenGL.framework/Versions/A/Libraries/libGL.dylib
    0x7fff4254a000 -     0x7fff4257eff7  libGLImage.dylib (17.10.22) <9A3FE633-61B8-3CC7-8183-62960109401A> /System/Library/Frameworks/OpenGL.framework/Versions/A/Libraries/libGLImage.dylib
    0x7fff42714000 -     0x7fff42750fff  libGLU.dylib (17.10.22) <D8B4D804-7323-30BC-871C-B7236FFC2FE3> /System/Library/Frameworks/OpenGL.framework/Versions/A/Libraries/libGLU.dylib
    0x7fff4318c000 -     0x7fff4319bff7  com.apple.opengl (17.10.22 - 17.10.22) <D3C57A32-6BD0-3228-B1C4-0F42A6128A6C> /System/Library/Frameworks/OpenGL.framework/Versions/A/OpenGL
    0x7fff44159000 -     0x7fff443dcffb  com.apple.QuartzCore (1.11 - 841.4) <FE927B0E-BD49-32CC-8A55-90F553C86C15> /System/Library/Frameworks/QuartzCore.framework/Versions/A/QuartzCore
    0x7fff44f5f000 -     0x7fff452a8ff1  com.apple.security (7.0 - 59306.140.5) <B6F8368F-2395-379B-B768-71C53BB1B903> /System/Library/Frameworks/Security.framework/Versions/A/Security
    0x7fff452a9000 -     0x7fff45331ffb  com.apple.securityfoundation (6.0 - 55236.60.1) <7C69DF47-4017-3DF2-B55B-712B481654CB> /System/Library/Frameworks/SecurityFoundation.framework/Versions/A/SecurityFoundation
    0x7fff45360000 -     0x7fff45364ff8  com.apple.xpc.ServiceManagement (1.0 - 1) <9B36FD0E-D280-35EB-ABAB-6AC5D7B2118F> /System/Library/Frameworks/ServiceManagement.framework/Versions/A/ServiceManagement
    0x7fff46010000 -     0x7fff4608aff7  com.apple.SystemConfiguration (1.19 - 1.19) <84F9B3BB-F7AF-3B7C-8CD0-D3C22D19619F> /System/Library/Frameworks/SystemConfiguration.framework/Versions/A/SystemConfiguration
    0x7fff49ffa000 -     0x7fff4a0bffe7  com.apple.APFS (1412.141.1 - 1412.141.1) <C86A3423-E61C-335A-9D17-0B3CE5BB6467> /System/Library/PrivateFrameworks/APFS.framework/Versions/A/APFS
    0x7fff4b1d4000 -     0x7fff4b1d5ff1  com.apple.AggregateDictionary (1.0 - 1) <95A291F5-B69F-3C37-9483-C3B2EBF52AC1> /System/Library/PrivateFrameworks/AggregateDictionary.framework/Versions/A/AggregateDictionary
    0x7fff4bc6b000 -     0x7fff4bc8fffb  com.apple.framework.Apple80211 (13.0 - 1610.1) <D94E03E8-4C38-3B2F-8DF4-473ACC5A7D71> /System/Library/PrivateFrameworks/Apple80211.framework/Versions/A/Apple80211
    0x7fff4bf4d000 -     0x7fff4bf5cfd7  com.apple.AppleFSCompression (119.100.1 - 1.0) <466ABD77-2E52-36D1-8E39-77AE2CC61611> /System/Library/PrivateFrameworks/AppleFSCompression.framework/Versions/A/AppleFSCompression
    0x7fff4c05b000 -     0x7fff4c066ff7  com.apple.AppleIDAuthSupport (1.0 - 1) <74F6CD9C-27A7-39C7-A7EB-47E60D2517EB> /System/Library/PrivateFrameworks/AppleIDAuthSupport.framework/Versions/A/AppleIDAuthSupport
    0x7fff4c0a8000 -     0x7fff4c0f0ff7  com.apple.AppleJPEG (1.0 - 1) <6DE30A07-C627-319B-A0DE-EB7A832BEB88> /System/Library/PrivateFrameworks/AppleJPEG.framework/Versions/A/AppleJPEG
    0x7fff4c4df000 -     0x7fff4c501fff  com.apple.applesauce (1.0 - 16.25) <68E0364C-AEA7-3654-A030-136BF3CD92F3> /System/Library/PrivateFrameworks/AppleSauce.framework/Versions/A/AppleSauce
    0x7fff4c5c0000 -     0x7fff4c5c3fff  com.apple.AppleSystemInfo (3.1.5 - 3.1.5) <67255151-F989-39F0-BC87-0C0BDAE70730> /System/Library/PrivateFrameworks/AppleSystemInfo.framework/Versions/A/AppleSystemInfo
    0x7fff4c65d000 -     0x7fff4c66cff9  com.apple.AssertionServices (1.0 - 223.140.2) <48AD21CA-B81D-380E-A04F-90C48FDA5203> /System/Library/PrivateFrameworks/AssertionServices.framework/Versions/A/AssertionServices
    0x7fff4d200000 -     0x7fff4d440fe8  com.apple.audio.AudioToolboxCore (1.0 - 1104.95) <9DB96FE2-AE60-32AE-B706-546E25BAE53F> /System/Library/PrivateFrameworks/AudioToolboxCore.framework/Versions/A/AudioToolboxCore
    0x7fff4d444000 -     0x7fff4d560fff  com.apple.AuthKit (1.0 - 1) <DC1A27C5-0172-3C72-9B24-06996D0B6207> /System/Library/PrivateFrameworks/AuthKit.framework/Versions/A/AuthKit
    0x7fff4d71d000 -     0x7fff4d726ff7  com.apple.coreservices.BackgroundTaskManagement (1.0 - 104) <A6877DAD-8F47-363C-983A-DC8DDE83B7B5> /System/Library/PrivateFrameworks/BackgroundTaskManagement.framework/Versions/A/BackgroundTaskManagement
    0x7fff4d727000 -     0x7fff4d7c8ff5  com.apple.backup.framework (1.11.7 - 1298.7.1) <C9DC35FA-E69F-3C64-9519-494126096337> /System/Library/PrivateFrameworks/Backup.framework/Versions/A/Backup
    0x7fff4d7c9000 -     0x7fff4d855ff6  com.apple.BaseBoard (466.3 - 466.3) <10D0F3BB-E8F3-365E-8528-6AC996A9B0E7> /System/Library/PrivateFrameworks/BaseBoard.framework/Versions/A/BaseBoard
    0x7fff4d957000 -     0x7fff4d993ff7  com.apple.bom (14.0 - 219.2) <79CBE5E7-054F-377B-9566-A86A9F120CF1> /System/Library/PrivateFrameworks/Bom.framework/Versions/A/Bom
    0x7fff4f40f000 -     0x7fff4f41fffb  com.apple.CommonAuth (4.0 - 2.0) <CF67FF34-4238-3ECA-B4A4-EA04F18A0D36> /System/Library/PrivateFrameworks/CommonAuth.framework/Versions/A/CommonAuth
    0x7fff4f433000 -     0x7fff4f44afff  com.apple.commonutilities (8.0 - 900) <F4C97244-E5D8-3F7D-8D94-4B6841C5A4EC> /System/Library/PrivateFrameworks/CommonUtilities.framework/Versions/A/CommonUtilities
    0x7fff4ff77000 -     0x7fff4ff98ff4  com.apple.analyticsd (1.0 - 1) <2162671C-D49D-3891-AB69-9EEB1FA47DD8> /System/Library/PrivateFrameworks/CoreAnalytics.framework/Versions/A/CoreAnalytics
    0x7fff5052f000 -     0x7fff5053fff3  com.apple.CoreEmoji (1.0 - 107.1) <7C2B3259-083B-31B8-BCDB-1BA360529936> /System/Library/PrivateFrameworks/CoreEmoji.framework/Versions/A/CoreEmoji
    0x7fff50b7f000 -     0x7fff50be9ff0  com.apple.CoreNLP (1.0 - 213) <E70E2505-8078-324E-BAE1-01A2DA980E2C> /System/Library/PrivateFrameworks/CoreNLP.framework/Versions/A/CoreNLP
    0x7fff51017000 -     0x7fff5101fff8  com.apple.CorePhoneNumbers (1.0 - 1) <E4DAD514-0B3B-3E0B-8AEA-39B320FAAF03> /System/Library/PrivateFrameworks/CorePhoneNumbers.framework/Versions/A/CorePhoneNumbers
    0x7fff51a0c000 -     0x7fff51a2ffff  com.apple.CoreSVG (1.0 - 129.3) <F38189F9-C8F9-3D62-9D5F-3F520FB81724> /System/Library/PrivateFrameworks/CoreSVG.framework/Versions/A/CoreSVG
    0x7fff51a64000 -     0x7fff51a92ffd  com.apple.CSStore (1069.24 - 1069.24) <C2D67667-FA0B-3DB6-AA34-6999EE4346A0> /System/Library/PrivateFrameworks/CoreServicesStore.framework/Versions/A/CoreServicesStore
    0x7fff520e5000 -     0x7fff52211ff6  com.apple.coreui (2.1 - 609.4) <788818B7-7EBC-316D-9464-D12E365E3791> /System/Library/PrivateFrameworks/CoreUI.framework/Versions/A/CoreUI
    0x7fff52212000 -     0x7fff523cbffa  com.apple.CoreUtils (6.2.4 - 624.7) <A74A1C65-6695-3F57-B703-0DEDE13E66C1> /System/Library/PrivateFrameworks/CoreUtils.framework/Versions/A/CoreUtils
    0x7fff52505000 -     0x7fff52518ff1  com.apple.CrashReporterSupport (10.13 - 15016) <ADF138F0-0274-3BA2-A1D2-48B91577FE53> /System/Library/PrivateFrameworks/CrashReporterSupport.framework/Versions/A/CrashReporterSupport
    0x7fff525d1000 -     0x7fff525e3ff8  com.apple.framework.DFRFoundation (1.0 - 252.50.1) <8162057E-E856-3451-9160-04AEDDECFFA4> /System/Library/PrivateFrameworks/DFRFoundation.framework/Versions/A/DFRFoundation
    0x7fff525e4000 -     0x7fff525e9fff  com.apple.DSExternalDisplay (3.1 - 380) <31ECB5FD-7660-33DB-BC5B-2B2A2AA7C686> /System/Library/PrivateFrameworks/DSExternalDisplay.framework/Versions/A/DSExternalDisplay
    0x7fff52673000 -     0x7fff526edff0  com.apple.datadetectorscore (8.0 - 659) <B1534796-1000-3520-A641-A97A4AC5D39B> /System/Library/PrivateFrameworks/DataDetectorsCore.framework/Versions/A/DataDetectorsCore
    0x7fff52777000 -     0x7fff528ffff6  com.apple.desktopservices (1.14.6 - 1281.6.1) <C2355E6B-C5F7-3E39-B778-B117BD4652C6> /System/Library/PrivateFrameworks/DesktopServicesPriv.framework/Versions/A/DesktopServicesPriv
    0x7fff542c0000 -     0x7fff546dbff1  com.apple.vision.FaceCore (4.3.0 - 4.3.0) <5D32F65D-2CD7-3204-975C-F4C9256E505F> /System/Library/PrivateFrameworks/FaceCore.framework/Versions/A/FaceCore
    0x7fff54d7a000 -     0x7fff54eb1ff4  libFontParser.dylib (277.2.6.3) <D93AD0C8-4657-3A3B-87EB-3DF3D522C70C> /System/Library/PrivateFrameworks/FontServices.framework/libFontParser.dylib
    0x7fff54f4a000 -     0x7fff54f5aff6  libhvf.dylib (1.0 - $[CURRENT_PROJECT_VERSION]) <C4B38245-337D-3553-9669-75E5D90071AE> /System/Library/PrivateFrameworks/FontServices.framework/libhvf.dylib
    0x7fff59af6000 -     0x7fff59afcfff  com.apple.GPUWrangler (5.2.7 - 5.2.7) <FA34760B-4E5C-3A18-A6C3-DBA68F9D1220> /System/Library/PrivateFrameworks/GPUWrangler.framework/Versions/A/GPUWrangler
    0x7fff5af6f000 -     0x7fff5af7dffb  com.apple.GraphVisualizer (1.0 - 100.1) <507D5812-9CB4-3C94-938C-59ED2B370818> /System/Library/PrivateFrameworks/GraphVisualizer.framework/Versions/A/GraphVisualizer
    0x7fff5b11c000 -     0x7fff5b1daff4  com.apple.Heimdal (4.0 - 2.0) <B86FE9DB-71BB-3B6E-A4AE-2B0B44570A7F> /System/Library/PrivateFrameworks/Heimdal.framework/Versions/A/Heimdal
    0x7fff5d366000 -     0x7fff5d36eff5  com.apple.IOAccelerator (438.7.3 - 438.7.3) <06E3E70B-C0D0-39A2-96B7-12ED6A0EBEE7> /System/Library/PrivateFrameworks/IOAccelerator.framework/Versions/A/IOAccelerator
    0x7fff5d37b000 -     0x7fff5d392fff  com.apple.IOPresentment (47.10 - 37) <32F1B3BC-4644-3982-AAB2-8EB5D5FF0161> /System/Library/PrivateFrameworks/IOPresentment.framework/Versions/A/IOPresentment
    0x7fff5d71a000 -     0x7fff5d765ff1  com.apple.IconServices (438.3 - 438.3) <0DADB4C3-46FF-3FDB-8A86-51E2067FC7F4> /System/Library/PrivateFrameworks/IconServices.framework/Versions/A/IconServices
    0x7fff5d923000 -     0x7fff5d92aff9  com.apple.InternationalSupport (1.0 - 45.4) <8D8D4A7D-FD35-36B8-A456-7C93030EDAB3> /System/Library/PrivateFrameworks/InternationalSupport.framework/Versions/A/InternationalSupport
    0x7fff5dbb7000 -     0x7fff5dbd6ffd  com.apple.security.KeychainCircle.KeychainCircle (1.0 - 1) <6F655A32-F963-3A7E-B475-E460F4AC7D99> /System/Library/PrivateFrameworks/KeychainCircle.framework/Versions/A/KeychainCircle
    0x7fff5dd0b000 -     0x7fff5ddd9ffd  com.apple.LanguageModeling (1.0 - 215.1) <C456087D-5B3A-390E-A665-862FA284C59C> /System/Library/PrivateFrameworks/LanguageModeling.framework/Versions/A/LanguageModeling
    0x7fff5ddda000 -     0x7fff5de22fff  com.apple.Lexicon-framework (1.0 - 72) <41F208B9-8255-3EC7-9673-FE0925D071D3> /System/Library/PrivateFrameworks/Lexicon.framework/Versions/A/Lexicon
    0x7fff5de29000 -     0x7fff5de2eff3  com.apple.LinguisticData (1.0 - 353.18) <3B92F249-4602-325F-984B-D2DE61EEE4E1> /System/Library/PrivateFrameworks/LinguisticData.framework/Versions/A/LinguisticData
    0x7fff5f197000 -     0x7fff5f1e3fff  com.apple.spotlight.metadata.utilities (1.0 - 2076.7) <0237323B-EC78-3FBF-9FC7-5A1FE2B5CE25> /System/Library/PrivateFrameworks/MetadataUtilities.framework/Versions/A/MetadataUtilities
    0x7fff5f1e4000 -     0x7fff5f2b5ffa  com.apple.gpusw.MetalTools (1.0 - 1) <99876E08-37D7-3828-8796-56D90C9AFBDB> /System/Library/PrivateFrameworks/MetalTools.framework/Versions/A/MetalTools
    0x7fff5f4e9000 -     0x7fff5f507fff  com.apple.MobileKeyBag (2.0 - 1.0) <D5FA7041-297F-3ADC-8C7A-6EAAAB82EB68> /System/Library/PrivateFrameworks/MobileKeyBag.framework/Versions/A/MobileKeyBag
    0x7fff5f76a000 -     0x7fff5f79aff7  com.apple.MultitouchSupport.framework (3440.1 - 3440.1) <6794E1C8-9627-33DF-84F4-FDD02C97F383> /System/Library/PrivateFrameworks/MultitouchSupport.framework/Versions/A/MultitouchSupport
    0x7fff5fc9a000 -     0x7fff5fca4fff  com.apple.NetAuth (6.2 - 6.2) <B0C03C41-87A3-352B-B130-96E1A6F94B47> /System/Library/PrivateFrameworks/NetAuth.framework/Versions/A/NetAuth
    0x7fff606b0000 -     0x7fff606fbffb  com.apple.OTSVG (1.0 - 643.1.5.2) <AD1D4601-05DE-37A7-AD7E-FCF46BF9981D> /System/Library/PrivateFrameworks/OTSVG.framework/Versions/A/OTSVG
    0x7fff61918000 -     0x7fff61923ff2  com.apple.PerformanceAnalysis (1.243.2 - 243.2) <B47C00E5-ECC2-313D-93D4-DBDF562C48EF> /System/Library/PrivateFrameworks/PerformanceAnalysis.framework/Versions/A/PerformanceAnalysis
    0x7fff61924000 -     0x7fff6194cffb  com.apple.persistentconnection (1.0 - 1.0) <5B2D87A8-2641-3F6D-ACEA-96B00F85AAB5> /System/Library/PrivateFrameworks/PersistentConnection.framework/Versions/A/PersistentConnection
    0x7fff6430c000 -     0x7fff64325ffb  com.apple.ProtocolBuffer (1 - 274.24.9.16.3) <5A020941-C43C-303E-8DE8-230FC6A84DBC> /System/Library/PrivateFrameworks/ProtocolBuffer.framework/Versions/A/ProtocolBuffer
    0x7fff64785000 -     0x7fff647aeff1  com.apple.RemoteViewServices (2.0 - 148) <D3AAC2BE-3423-3F18-9654-E35F1DD8DDB3> /System/Library/PrivateFrameworks/RemoteViewServices.framework/Versions/A/RemoteViewServices
    0x7fff64913000 -     0x7fff6494eff0  com.apple.RunningBoardServices (1.0 - 223.140.2) <96BB04BD-D6E0-3D70-8F36-89B46DA1DA30> /System/Library/PrivateFrameworks/RunningBoardServices.framework/Versions/A/RunningBoardServices
    0x7fff663a5000 -     0x7fff664ccfff  com.apple.Sharing (1526.37 - 1526.37) <CBDA0ADD-F1E7-3B06-9118-C5E183F0D3D6> /System/Library/PrivateFrameworks/Sharing.framework/Versions/A/Sharing
    0x7fff678e1000 -     0x7fff67bd7ff7  com.apple.SkyLight (1.600.0 - 451.4) <A24929C3-95E6-35A7-9654-46FF3F4D1E80> /System/Library/PrivateFrameworks/SkyLight.framework/Versions/A/SkyLight
    0x7fff68424000 -     0x7fff68432ffb  com.apple.SpeechRecognitionCore (6.0.91.2 - 6.0.91.2) <4D6CAC2A-151B-3BBE-BDB7-E2BE72128691> /System/Library/PrivateFrameworks/SpeechRecognitionCore.framework/Versions/A/SpeechRecognitionCore
    0x7fff68f26000 -     0x7fff68f36ff3  com.apple.TCC (1.0 - 1) <C9EB52E3-099B-3597-9623-067C403FA525> /System/Library/PrivateFrameworks/TCC.framework/Versions/A/TCC
    0x7fff6945b000 -     0x7fff69521ff0  com.apple.TextureIO (3.10.9 - 3.10.9) <EEDAB753-329A-396A-8119-5BEDF7DB5A56> /System/Library/PrivateFrameworks/TextureIO.framework/Versions/A/TextureIO
    0x7fff696f1000 -     0x7fff69949ff0  com.apple.UIFoundation (1.0 - 662) <EC55B9E5-7E62-380A-9AB1-FC7BEF663653> /System/Library/PrivateFrameworks/UIFoundation.framework/Versions/A/UIFoundation
    0x7fff6b61c000 -     0x7fff6b61dfff  com.apple.WatchdogClient.framework (1.0 - 67.120.2) <FFA17DA1-F6DD-34D3-A708-1F73C8BA7EA7> /System/Library/PrivateFrameworks/WatchdogClient.framework/Versions/A/WatchdogClient
    0x7fff6c24d000 -     0x7fff6c250ffa  com.apple.dt.XCTTargetBootstrap (1.0 - 16091) <D459D628-58C5-39A6-B7E8-B691CBEECEC1> /System/Library/PrivateFrameworks/XCTTargetBootstrap.framework/Versions/A/XCTTargetBootstrap
    0x7fff6c2ca000 -     0x7fff6c2d8ff5  com.apple.audio.caulk (1.0 - 32.3) <06D695EA-E2BC-31E4-9816-9C12542BA744> /System/Library/PrivateFrameworks/caulk.framework/Versions/A/caulk
    0x7fff6c61a000 -     0x7fff6c61cff3  com.apple.loginsupport (1.0 - 1) <12F77885-27DC-3837-9CE9-A25EBA75F833> /System/Library/PrivateFrameworks/login.framework/Versions/A/Frameworks/loginsupport.framework/Versions/A/loginsupport
    0x7fff6f100000 -     0x7fff6f133ffa  libAudioToolboxUtility.dylib (1104.95) <E534364D-5E5F-37BA-9FB6-FFFF1416820C> /usr/lib/libAudioToolboxUtility.dylib
    0x7fff6f13a000 -     0x7fff6f16efff  libCRFSuite.dylib (48) <5E5DE3CB-30DD-34DC-AEF8-FE8536A85E96> /usr/lib/libCRFSuite.dylib
    0x7fff6f171000 -     0x7fff6f17bfff  libChineseTokenizer.dylib (34) <7F0DA183-1796-315A-B44A-2C234C7C50BE> /usr/lib/libChineseTokenizer.dylib
    0x7fff6f207000 -     0x7fff6f209ff7  libDiagnosticMessagesClient.dylib (112) <C94F3B7B-1854-38EB-9778-834501C53B3F> /usr/lib/libDiagnosticMessagesClient.dylib
    0x7fff6f24f000 -     0x7fff6f406ffb  libFosl_dynamic.dylib (100.4) <737573B2-190A-3BA1-8220-807AD0A2CE5E> /usr/lib/libFosl_dynamic.dylib
    0x7fff6f42d000 -     0x7fff6f433ff3  libIOReport.dylib (54) <75D177C4-BAD7-3285-B8E1-3019F49B3178> /usr/lib/libIOReport.dylib
    0x7fff6f54b000 -     0x7fff6f56bff7  libMobileGestalt.dylib (826.140.5) <2BE94E6A-FA61-312F-84A1-F764D71B7E39> /usr/lib/libMobileGestalt.dylib
    0x7fff6f6dd000 -     0x7fff6f6defff  libSystem.B.dylib (1281.100.1) <8E6AD412-91E7-36FC-A6FD-C13B06A4952A> /usr/lib/libSystem.B.dylib
    0x7fff6f76b000 -     0x7fff6f76cfff  libThaiTokenizer.dylib (3) <4F4ADE99-0D09-3223-B7C0-C407AB6DE8DC> /usr/lib/libThaiTokenizer.dylib
    0x7fff6f784000 -     0x7fff6f79afff  libapple_nghttp2.dylib (1.39.2) <07FEC48A-87CF-32A3-8194-FA70B361713A> /usr/lib/libapple_nghttp2.dylib
    0x7fff6f7cf000 -     0x7fff6f841ff7  libarchive.2.dylib (72.140.2) <F9EA2883-5D5C-3FA6-B3F8-C5031BF88ABD> /usr/lib/libarchive.2.dylib
    0x7fff6f842000 -     0x7fff6f8dbfe5  libate.dylib (3.0.1) <76EA60FB-748C-313F-8951-B076540BEA97> /usr/lib/libate.dylib
    0x7fff6f8df000 -     0x7fff6f8dfff3  libauto.dylib (187) <B6124448-7690-34AE-8939-ED84AAC630CE> /usr/lib/libauto.dylib
    0x7fff6f9a5000 -     0x7fff6f9b5ffb  libbsm.0.dylib (60.100.1) <00BFFB9A-2FFE-3C24-896A-251BC61917FD> /usr/lib/libbsm.0.dylib
    0x7fff6f9b6000 -     0x7fff6f9c2fff  libbz2.1.0.dylib (44) <14CC4988-B6D4-3879-AFC2-9A0DDC6388DE> /usr/lib/libbz2.1.0.dylib
    0x7fff6f9c3000 -     0x7fff6fa15fff  libc++.1.dylib (902.1) <59A8239F-C28A-3B59-B8FA-11340DC85EDC> /usr/lib/libc++.1.dylib
    0x7fff6fa16000 -     0x7fff6fa2bffb  libc++abi.dylib (902) <E692F14F-C65E-303B-9921-BB7E97D77855> /usr/lib/libc++abi.dylib
    0x7fff6fa2c000 -     0x7fff6fa2cfff  libcharset.1.dylib (59) <72447768-9244-39AB-8E79-2FA14EC0AD33> /usr/lib/libcharset.1.dylib
    0x7fff6fa2d000 -     0x7fff6fa3efff  libcmph.dylib (8) <E72A20DB-2E86-378D-A237-EB9A1370F989> /usr/lib/libcmph.dylib
    0x7fff6fa3f000 -     0x7fff6fa56fd7  libcompression.dylib (87) <64C91066-586D-38C0-A2F3-3E60A940F859> /usr/lib/libcompression.dylib
    0x7fff6fd30000 -     0x7fff6fd46ff7  libcoretls.dylib (167) <770A5B96-936E-34E3-B006-B1CEC299B5A5> /usr/lib/libcoretls.dylib
    0x7fff6fd47000 -     0x7fff6fd48fff  libcoretls_cfhelpers.dylib (167) <940BF370-FD0C-30A8-AA05-FF48DA44FA4C> /usr/lib/libcoretls_cfhelpers.dylib
    0x7fff70305000 -     0x7fff70364ff7  libcups.2.dylib (483.7) <821ED293-B7B3-3B37-88C9-7B6CA91DA7FA> /usr/lib/libcups.2.dylib
    0x7fff7046e000 -     0x7fff7046efff  libenergytrace.dylib (21) <162DFCC0-8F48-3DD0-914F-FA8653E27B26> /usr/lib/libenergytrace.dylib
    0x7fff7046f000 -     0x7fff70487fff  libexpat.1.dylib (19.60.2) <FED7C38B-92D8-342D-AED7-871B12D1F7E7> /usr/lib/libexpat.1.dylib
    0x7fff70495000 -     0x7fff70497fff  libfakelink.dylib (149.1) <36146CB2-E6A5-37BB-9EE8-1B4034D8F3AD> /usr/lib/libfakelink.dylib
    0x7fff704a6000 -     0x7fff704abfff  libgermantok.dylib (24) <D2AE5AC0-EDCE-3216-B8C9-CF59292A545F> /usr/lib/libgermantok.dylib
    0x7fff704ac000 -     0x7fff704b5ff7  libheimdal-asn1.dylib (564.140.1) <0AC6FB62-2B0F-3E93-A931-E4DC4B1D757A> /usr/lib/libheimdal-asn1.dylib
    0x7fff704b6000 -     0x7fff705a6fff  libiconv.2.dylib (59) <18311A67-E4EF-3CC7-95B3-C0EDEE3A282F> /usr/lib/libiconv.2.dylib
    0x7fff705a7000 -     0x7fff707fefff  libicucore.A.dylib (64260.0.1) <8AC2CB07-E7E0-340D-A849-186FA1F27251> /usr/lib/libicucore.A.dylib
    0x7fff70816000 -     0x7fff70817fff  liblangid.dylib (133) <30CFC08C-EF36-3CF5-8AEA-C1CB070306B7> /usr/lib/liblangid.dylib
    0x7fff70818000 -     0x7fff70830ff3  liblzma.5.dylib (16) <C131EF18-2CDD-3271-8A30-A8760D4FE166> /usr/lib/liblzma.5.dylib
    0x7fff70848000 -     0x7fff708efff7  libmecab.dylib (883.11) <0D5BFD01-D4A7-3C8D-AA69-C329C1A69792> /usr/lib/libmecab.dylib
    0x7fff708f0000 -     0x7fff70b52ff1  libmecabra.dylib (883.11) <E31DE74D-1B88-377F-ACD3-D789D29C3AE7> /usr/lib/libmecabra.dylib
    0x7fff70ebf000 -     0x7fff70eeefff  libncurses.5.4.dylib (57) <995DFEEA-40F3-377F-B73D-D02AC59D591F> /usr/lib/libncurses.5.4.dylib
    0x7fff7101e000 -     0x7fff7149aff5  libnetwork.dylib (1880.120.4) <BA294A54-F309-398D-B308-F97032AFF555> /usr/lib/libnetwork.dylib
    0x7fff7153b000 -     0x7fff7156efde  libobjc.A.dylib (787.1) <6DF81160-5E7F-3E31-AA1E-C875E3B98AF6> /usr/lib/libobjc.A.dylib
    0x7fff71581000 -     0x7fff71585fff  libpam.2.dylib (25.100.1) <0502F395-8EE6-3D2A-9239-06FD5622E19E> /usr/lib/libpam.2.dylib
    0x7fff71588000 -     0x7fff715beff7  libpcap.A.dylib (89.120.1) <A76EC076-A8EA-354C-B95F-7AB1EAFBCC65> /usr/lib/libpcap.A.dylib
    0x7fff71642000 -     0x7fff7165afff  libresolv.9.dylib (67.40.1) <C57EDFEF-D36A-310B-8D14-8C68A625B1E8> /usr/lib/libresolv.9.dylib
    0x7fff716b6000 -     0x7fff718a0ff7  libsqlite3.dylib (308.5) <35A2BD9F-4E33-30DE-A994-4AB585AC3AFE> /usr/lib/libsqlite3.dylib
    0x7fff71af1000 -     0x7fff71af4ffb  libutil.dylib (57) <F01467F6-23A7-37EE-A170-33CE1577B41D> /usr/lib/libutil.dylib
    0x7fff71af5000 -     0x7fff71b02ff7  libxar.1.dylib (425.2) <EE964412-9E25-30B3-BCC0-CCEFBCC8094B> /usr/lib/libxar.1.dylib
    0x7fff71b08000 -     0x7fff71beafff  libxml2.2.dylib (33.7) <20567881-7204-3C11-9179-50FE34B3301B> /usr/lib/libxml2.2.dylib
    0x7fff71bee000 -     0x7fff71c16fff  libxslt.1.dylib (16.9) <34A45627-DA5B-37D2-9609-65B425E0010A> /usr/lib/libxslt.1.dylib
    0x7fff71c17000 -     0x7fff71c29ff3  libz.1.dylib (76) <793D9643-CD83-3AAC-8B96-88D548FAB620> /usr/lib/libz.1.dylib
    0x7fff724d8000 -     0x7fff724ddff3  libcache.dylib (83) <AF488D13-9E89-35E0-B078-BE37CC5B8586> /usr/lib/system/libcache.dylib
    0x7fff724de000 -     0x7fff724e9fff  libcommonCrypto.dylib (60165.120.1) <C7912BE5-993E-3581-B2A0-6AABDC8C5562> /usr/lib/system/libcommonCrypto.dylib
    0x7fff724ea000 -     0x7fff724f1fff  libcompiler_rt.dylib (101.2) <49B8F644-5705-3F16-BBE0-6FFF9B17C36E> /usr/lib/system/libcompiler_rt.dylib
    0x7fff724f2000 -     0x7fff724fbff7  libcopyfile.dylib (166.40.1) <3C481225-21E7-370A-A30E-0CCFDD64A92C> /usr/lib/system/libcopyfile.dylib
    0x7fff724fc000 -     0x7fff7258efdb  libcorecrypto.dylib (866.140.1) <60567BF8-80FA-359A-B2F3-A3BAEFB288FD> /usr/lib/system/libcorecrypto.dylib
    0x7fff7269b000 -     0x7fff726dbff0  libdispatch.dylib (1173.100.2) <CD9C059C-91D9-30E8-8926-5B9CD0D5D4F5> /usr/lib/system/libdispatch.dylib
    0x7fff726dc000 -     0x7fff72712fff  libdyld.dylib (750.6) <789A18C2-8AC7-3C88-813D-CD674376585D> /usr/lib/system/libdyld.dylib
    0x7fff72713000 -     0x7fff72713ffb  libkeymgr.dylib (30) <DB3337BE-01CA-3425-BD0C-87774FC0CDC0> /usr/lib/system/libkeymgr.dylib
    0x7fff72714000 -     0x7fff72720ff3  libkxld.dylib (6153.141.10) <11EABEB3-CD17-3787-86BE-B8B21817E89B> /usr/lib/system/libkxld.dylib
    0x7fff72721000 -     0x7fff72721ff7  liblaunch.dylib (1738.140.2) <7200E214-9B4D-3B22-9844-4C7892FC890B> /usr/lib/system/liblaunch.dylib
    0x7fff72722000 -     0x7fff72727ff7  libmacho.dylib (959.0.1) <AA613A9C-961A-3B67-B696-4622FA59FC4E> /usr/lib/system/libmacho.dylib
    0x7fff72728000 -     0x7fff7272aff3  libquarantine.dylib (110.40.3) <F234E51D-FD0B-3EE4-B679-AE3EE9C536C3> /usr/lib/system/libquarantine.dylib
    0x7fff7272b000 -     0x7fff7272cff7  libremovefile.dylib (48) <7C7EFC79-BD24-33EF-B073-06AED234593E> /usr/lib/system/libremovefile.dylib
    0x7fff7272d000 -     0x7fff72744ff3  libsystem_asl.dylib (377.60.2) <1563EE02-0657-3B78-99BE-A947C24122EF> /usr/lib/system/libsystem_asl.dylib
    0x7fff72745000 -     0x7fff72745ff7  libsystem_blocks.dylib (74) <0D53847E-AF5F-3ACF-B51F-A15DEA4DEC58> /usr/lib/system/libsystem_blocks.dylib
    0x7fff72746000 -     0x7fff727cdfff  libsystem_c.dylib (1353.100.2) <BBDED5E6-A646-3EED-B33A-91E4331EA063> /usr/lib/system/libsystem_c.dylib
    0x7fff727ce000 -     0x7fff727d1ffb  libsystem_configuration.dylib (1061.141.1) <0EE84C33-64FD-372B-974A-AF7A136F2068> /usr/lib/system/libsystem_configuration.dylib
    0x7fff727d2000 -     0x7fff727d5fff  libsystem_coreservices.dylib (114) <A199156E-058D-3ABB-BCE9-4B9F20DCED0F> /usr/lib/system/libsystem_coreservices.dylib
    0x7fff727d6000 -     0x7fff727defff  libsystem_darwin.dylib (1353.100.2) <5B12B5DB-3F30-37C1-8ECC-49A66B1F2864> /usr/lib/system/libsystem_darwin.dylib
    0x7fff727df000 -     0x7fff727e6fff  libsystem_dnssd.dylib (1096.100.3) <EBB4C2C2-E031-3094-B40A-E67BF261D295> /usr/lib/system/libsystem_dnssd.dylib
    0x7fff727e7000 -     0x7fff727e8ffb  libsystem_featureflags.dylib (17) <29FD922A-EC2C-3F25-BCCC-B58D716E60EC> /usr/lib/system/libsystem_featureflags.dylib
    0x7fff727e9000 -     0x7fff72836ff7  libsystem_info.dylib (538) <8A321605-5480-330B-AF9E-64E65DE61747> /usr/lib/system/libsystem_info.dylib
    0x7fff72837000 -     0x7fff72863ff7  libsystem_kernel.dylib (6153.141.10) <FF092EE8-5BEE-3B9A-8749-F0A067115C7E> /usr/lib/system/libsystem_kernel.dylib
    0x7fff72864000 -     0x7fff728abfff  libsystem_m.dylib (3178) <00F331F1-0D09-39B3-8736-1FE90E64E903> /usr/lib/system/libsystem_m.dylib
    0x7fff728ac000 -     0x7fff728d3fff  libsystem_malloc.dylib (283.100.6) <8549294E-4C53-36EB-99F3-584A7393D8D5> /usr/lib/system/libsystem_malloc.dylib
    0x7fff728d4000 -     0x7fff728e1ffb  libsystem_networkextension.dylib (1095.140.2) <F06C65C5-2CBE-313C-96E1-A09240F9FE57> /usr/lib/system/libsystem_networkextension.dylib
    0x7fff728e2000 -     0x7fff728ebff7  libsystem_notify.dylib (241.100.2) <FA22F928-D91B-3AA5-96BB-3186AC0FB264> /usr/lib/system/libsystem_notify.dylib
    0x7fff728ec000 -     0x7fff728f4fef  libsystem_platform.dylib (220.100.1) <009A7C1F-313A-318E-B9F2-30F4C06FEA5C> /usr/lib/system/libsystem_platform.dylib
    0x7fff728f5000 -     0x7fff728fffff  libsystem_pthread.dylib (416.100.3) <62CB1A98-0B8F-31E7-A02B-A1139927F61D> /usr/lib/system/libsystem_pthread.dylib
    0x7fff72900000 -     0x7fff72904ff3  libsystem_sandbox.dylib (1217.141.2) <051C4018-4345-3034-AC98-6DE42FB8273B> /usr/lib/system/libsystem_sandbox.dylib
    0x7fff72905000 -     0x7fff72907fff  libsystem_secinit.dylib (62.100.2) <F80872AA-E1FD-3D7E-8729-467656EC6561> /usr/lib/system/libsystem_secinit.dylib
    0x7fff72908000 -     0x7fff7290fffb  libsystem_symptoms.dylib (1238.120.2) <702D0910-5C34-3D43-9631-8BD215DE4FE1> /usr/lib/system/libsystem_symptoms.dylib
    0x7fff72910000 -     0x7fff72926ff2  libsystem_trace.dylib (1147.120.1) <BC141783-66D9-3137-A783-211B38E49ADB> /usr/lib/system/libsystem_trace.dylib
    0x7fff72928000 -     0x7fff7292dff7  libunwind.dylib (35.4) <42B7B509-BAFE-365B-893A-72414C92F5BF> /usr/lib/system/libunwind.dylib
    0x7fff7292e000 -     0x7fff72963ffe  libxpc.dylib (1738.140.2) <54EEF402-42C7-3995-BADE-93C48EFC4452> /usr/lib/system/libxpc.dylib

External Modification Summary:
  Calls made by other processes targeting this process:
    task_for_pid: 0
    thread_create: 0
    thread_set_state: 0
  Calls made by this process:
    task_for_pid: 0
    thread_create: 0
    thread_set_state: 0
  Calls made by all processes on this machine:
    task_for_pid: 20153
    thread_create: 0
    thread_set_state: 0

VM Region Summary:
ReadOnly portion of Libraries: Total=546.0M resident=0K(0%) swapped_out_or_unallocated=546.0M(100%)
Writable regions: Total=539.6M written=0K(0%) resident=0K(0%) swapped_out=0K(0%) unallocated=539.6M(100%)
 
                                VIRTUAL   REGION 
REGION TYPE                        SIZE    COUNT (non-coalesced) 
===========                     =======  ======= 
Activity Tracing                   256K        1 
Kernel Alloc Once                    8K        1 
MALLOC                           147.2M       16 
MALLOC guard page                   16K        4 
MALLOC_NANO (reserved)           384.0M        1         reserved VM address space (unallocated)
STACK GUARD                       56.0M        1 
Stack                             8192K        1 
__DATA                            21.7M      239 
__DATA_CONST                        20K        1 
__FONT_DATA                          4K        1 
__LINKEDIT                       390.1M        3 
__OBJC_RO                         32.3M        1 
__OBJC_RW                         1908K        2 
__TEXT                           155.9M      243 
__UNICODE                          564K        1 
shared memory                       12K        3 
===========                     =======  ======= 
TOTAL                              1.2G      519 
TOTAL, minus reserved VM space   813.9M      519 

Model: MacBookPro15,1, BootROM 1554.60.15.0.0 (iBridge: 18.16.13030.0.0,0), 6 processors, 6-Core Intel Core i7, 2,2 GHz, 16 GB, SMC 
Graphics: kHW_IntelUHDGraphics630Item, Intel UHD Graphics 630, spdisplays_builtin
Graphics: kHW_AMDRadeonPro555XItem, Radeon Pro 555X, spdisplays_pcie_device, 4 GB
Memory Module: BANK 0/ChannelA-DIMM0, 8 GB, DDR4, 2400 MHz, Micron, 8ATF1G64HZ-2G6E1
Memory Module: BANK 2/ChannelB-DIMM0, 8 GB, DDR4, 2400 MHz, Micron, 8ATF1G64HZ-2G6E1
AirPort: spairport_wireless_card_type_airport_extreme (0x14E4, 0x7BF), wl0: Oct 28 2020 13:06:41 version 9.30.357.42.32.5.48 FWID 01-4f9e2d7c
Bluetooth: Version 7.0.6f8, 3 services, 27 devices, 1 incoming serial ports
Network Service: Wi-Fi, AirPort, en0
USB Device: USB 3.1 Bus
USB Device: Apple T2 Bus
USB Device: Touch Bar Backlight
USB Device: Touch Bar Display
USB Device: Apple Internal Keyboard / Trackpad
USB Device: Headset
USB Device: Ambient Light Sensor
USB Device: FaceTime HD Camera (Built-in)
USB Device: Apple T2 Controller
Thunderbolt Bus: MacBook Pro, Apple Inc., 47.4
Thunderbolt Bus: MacBook Pro, Apple Inc., 47.4
