# DRM

### dynamic analyzing

it's a PE dll file

## stack

initializing an 32-bit exe.

   ```Text
    wow64cpu.dll!TurboDispatchJumpAddressEnd+0x544
    wow64cpu.dll!TurboDispatchJumpAddressEnd+0x224
    wow64cpu.dll!TurboDispatchJumpAddressEnd+0x5c6
    wow64.dll!Wow64KiUserCallbackDispatcher+0x66d
    wow64.dll!Wow64LdrpInitialize+0x12d
    ntdll.dll!LdrInitShimEngineDynamic+0x309b
    ntdll.dll!RtlNotifyFeatureUsage+0x1cb1a
    ntdll.dll!LdrInitializeThunk+0xe3
    ntdll.dll!LdrInitializeThunk+0xe
   ```

DRM stack

   ```Text
    ntdll.dll!ZwReadFile+0xc
    ucrtbase.dll!_read+0xc16
    ucrtbase.dll!_read+0x8f
    ucrtbase.dll!fegetenv+0x156c
    ucrtbase.dll!fgetc+0x175
    ucrtbase.dll!getchar+0xa
    DRM.exe+0x1998
    KERNEL32.DLL!BaseThreadInitThunk+0x19
    ntdll.dll!RtlGetFullPathName_UEx+0x4bf
    ntdll.dll!RtlGetFullPathName_UEx+0x48d
   ```

### info

wow64cpu.dll - subsystem that runs 32-bit application on 64-bit windows systems
