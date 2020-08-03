//=== 2020.08.03
$ electronize build /target linux
PathName.music is ok

but
$ electronize buildstep1 /target win
Controllers/HomeController.cs(14,73): 
error CS0117: 'PathName' does not contain a definition for 'music'
--> ElectronNET.API.Entities.PathName

[Q] how to get system music folder in C#?
-->
 error CS1503: Argument 1: cannot convert from 
'System.Environment.SpecialFolder' to 'ElectronNET.API.Entities.PathName'

//===
$ dotnet build
$ dotnet run
...
info: Microsoft.AspNetCore.DataProtection.KeyManagement.XmlKeyManager[0]
      User profile is available. Using '~/.aspnet/DataProtection-Keys' as key repository; keys will not be encrypted at rest.
Hosting environment: Development
Content root path: /dotnetCore/electron.net-musicplayer-sample/MyElectronMusicPlayer
Now listening on: http://localhost:53037
Application started. Press Ctrl+C to shut down.
info: Microsoft.AspNetCore.Hosting.Diagnostics[1]
      Request starting HTTP/1.1 GET http://localhost:53037/
info: Microsoft.AspNetCore.Routing.EndpointMiddleware[0]
      Executing endpoint 'MyElectronMusicPlayer.Controllers.HomeController.Index (MyElectronMusicPlayer)'
info: Microsoft.AspNetCore.Mvc.Infrastructure.ControllerActionInvoker[3]
      Route matched with {action = "Index", controller = "Home"}. Executing controller action with signature System.Threading.Tasks.Task`1[Microsoft.AspNetCore.Mvc.IActionResult] Index() on controller MyElectronMusicPlayer.Controllers.HomeController (MyElectronMusicPlayer).

...

open another terminal
$ chromium-browser  http://localhost:53037
...
debug1: client_input_channel_open: ctype x11 rchan 3 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54226
debug1: channel 1: new [x11]
debug1: confirm x11
debug1: client_input_channel_open: ctype x11 rchan 4 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54228
debug1: channel 2: new [x11]
debug1: confirm x11
libGL error: No matching fbConfigs or visuals found
libGL error: failed to load driver: swrast
[2917:2917:0803/114941.137657:ERROR:edid_parser.cc(102)] Too short EDID data: manufacturer id
debug1: client_input_channel_open: ctype x11 rchan 5 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54230
debug1: channel 3: new [x11]
debug1: confirm x11
ATTENTION: default value of option force_s3tc_enable overridden by environment.
libGL error: No matching fbConfigs or visuals found
libGL error: failed to load driver: swrast
[2953:2953:0803/114942.066295:ERROR:viz_main_impl.cc(159)] Exiting GPU process due to errors during initializationdebug1: channel 3: FORCE input drain

debug1: channel 3: free: x11, nchannels 4
debug1: client_input_channel_open: ctype x11 rchan 5 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54232
debug1: channel 3: new [x11]
debug1: confirm x11
debug1: client_input_channel_open: ctype x11 rchan 6 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54234
debug1: channel 4: new [x11]
debug1: confirm x11
[2917:2973:0803/114943.447336:ERROR:bus.cc(393)] Failed to connect to the bus: Could not parse server address: Unknown address type (examples of valid types are "tcp" and on UNIX "unix")
[2917:2973:0803/114943.447708:ERROR:bus.cc(393)] Failed to connect to the bus: Could not parse server address: Unknown address type (examples of valid types are "tcp" and on UNIX "unix")
[2917:2973:0803/114944.522059:ERROR:bus.cc(393)] Failed to connect to the bus: Could not parse server address: Unknown address type (examples of valid types are "tcp" and on UNIX "unix")
[2917:2973:0803/114944.522534:ERROR:bus.cc(393)] Failed to connect to the bus: Could not parse server address: Unknown address type (examples of valid types are "tcp" and on UNIX "unix")
[2917:2917:0803/114945.816537:ERROR:browser_switcher_service.cc(238)] XXX Init()
debug1: client_input_channel_open: ctype x11 rchan 7 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54236
debug1: channel 5: new [x11]
debug1: confirm x11
debug1: channel 5: FORCE input drain
debug1: channel 5: free: x11, nchannels 6
debug1: client_input_channel_open: ctype x11 rchan 7 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54242
debug1: channel 5: new [x11]
debug1: confirm x11
debug1: channel 5: FORCE input drain
debug1: channel 5: free: x11, nchannels 6
debug1: client_input_channel_open: ctype x11 rchan 7 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54246
debug1: channel 5: new [x11]
debug1: confirm x11
debug1: channel 5: FORCE input drain
debug1: client_input_channel_open: ctype x11 rchan 8 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54248
debug1: channel 6: new [x11]
debug1: confirm x11
debug1: channel 5: free: x11, nchannels 7
debug1: channel 6: FORCE input drain
debug1: channel 6: free: x11, nchannels 6
debug1: client_input_channel_open: ctype x11 rchan 7 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54250
debug1: channel 5: new [x11]
debug1: confirm x11
debug1: channel 5: FORCE input drain
debug1: channel 5: free: x11, nchannels 6
debug1: client_input_channel_open: ctype x11 rchan 7 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54252
debug1: channel 5: new [x11]
debug1: confirm x11
debug1: channel 5: FORCE input drain
debug1: channel 5: free: x11, nchannels 6
debug1: client_input_channel_open: ctype x11 rchan 7 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54254
debug1: channel 5: new [x11]
debug1: confirm x11
debug1: channel 5: FORCE input drain
debug1: channel 5: free: x11, nchannels 6
debug1: client_input_channel_open: ctype x11 rchan 7 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54256
debug1: channel 5: new [x11]
debug1: confirm x11
debug1: channel 5: FORCE input drain
debug1: channel 5: free: x11, nchannels 6
../../sandbox/linux/seccomp-bpf-helpers/sigsys_handlers.cc:**CRASHING**:seccomp-bpf failure in syscall 0063
debug1: channel 4: FORCE input drain
debug1: channel 3: FORCE input drain
debug1: channel 3: free: x11, nchannels 5
debug1: channel 4: free: x11, nchannels 4
debug1: client_input_channel_open: ctype x11 rchan 5 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54258
debug1: channel 3: new [x11]
debug1: confirm x11
debug1: client_input_channel_open: ctype x11 rchan 6 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54260
debug1: channel 4: new [x11]
debug1: confirm x11
../../sandbox/linux/seccomp-bpf-helpers/sigsys_handlers.cc:**CRASHING**:seccomp-bpf failure in syscall 0063
debug1: channel 4: FORCE input drain
debug1: channel 3: FORCE input drain
debug1: channel 3: free: x11, nchannels 5
debug1: channel 4: free: x11, nchannels 4
debug1: client_input_channel_open: ctype x11 rchan 5 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54262
debug1: channel 3: new [x11]
debug1: confirm x11
debug1: client_input_channel_open: ctype x11 rchan 6 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54264
debug1: channel 4: new [x11]
debug1: confirm x11
../../sandbox/linux/seccomp-bpf-helpers/sigsys_handlers.cc:**CRASHING**:seccomp-bpf failure in syscall 0063
debug1: channel 4: FORCE input drain
debug1: channel 3: FORCE input drain
debug1: channel 4: free: x11, nchannels 5
debug1: channel 3: free: x11, nchannels 4
debug1: client_input_channel_open: ctype x11 rchan 5 win 65536 max 16384
debug1: client_request_x11: request from 127.0.0.1 54266
debug1: channel 3: new [x11]
debug1: confirm x11
[3088:3088:0803/114948.367111:ERROR:sandbox_linux.cc(374)] InitializeSandbox() called with multiple threads in process gpu-process.
Xlib:  extension "MIT-SHM" missing on display "U16x64:11.0".
debug1: SSH2_MSG_KEXINIT received
debug1: SSH2_MSG_KEXINIT sent
debug1: kex: algorithm: curve25519-sha256@libssh.org
debug1: kex: host key algorithm: ecdsa-sha2-nistp256
debug1: kex: server->client cipher: chacha20-poly1305@openssh.com MAC: <implicit> compression: none
debug1: kex: client->server cipher: chacha20-poly1305@openssh.com MAC: <implicit> compression: none
debug1: expecting SSH2_MSG_KEX_ECDH_REPLY
debug1: rekeying in progress
debug1: rekeying in progress
debug1: Server host key: ecdsa-sha2-nistp256 SHA256:XR7rAZ7Nc73FWhhI15ezsYftiyM0+QUza17v3ExjJtc
debug1: set_newkeys: rekeying, input 1073881984 bytes 134202024 blocks, output 535228 bytes 58567 blocks
debug1: rekey after 134217728 blocks
debug1: SSH2_MSG_NEWKEYS sent
debug1: expecting SSH2_MSG_NEWKEYS
debug1: SSH2_MSG_NEWKEYS received
debug1: set_newkeys: rekeying, input 1073881996 bytes 134202025 blocks, output 535228 bytes 0 blocks
debug1: rekey after 134217728 blocks
debug1: SSH2_MSG_KEXINIT received
debug1: SSH2_MSG_KEXINIT sent
debug1: kex: algorithm: curve25519-sha256@libssh.org
debug1: kex: host key algorithm: ecdsa-sha2-nistp256
debug1: kex: server->client cipher: chacha20-poly1305@openssh.com MAC: <implicit> compression: none
debug1: kex: client->server cipher: chacha20-poly1305@openssh.com MAC: <implicit> compression: none
debug1: expecting SSH2_MSG_KEX_ECDH_REPLY
debug1: rekeying in progress
debug1: rekeying in progress
debug1: Server host key: ecdsa-sha2-nistp256 SHA256:XR7rAZ7Nc73FWhhI15ezsYftiyM0+QUza17v3ExjJtc
debug1: set_newkeys: rekeying, input 2147761112 bytes 134202155 blocks, output 859492 bytes 32708 blocks
debug1: rekey after 134217728 blocks
debug1: SSH2_MSG_NEWKEYS sent
debug1: expecting SSH2_MSG_NEWKEYS
debug1: SSH2_MSG_NEWKEYS received
debug1: set_newkeys: rekeying, input 2147761124 bytes 134202156 blocks, output 859492 bytes 0 blocks
debug1: rekey after 134217728 blocks
debug1: SSH2_MSG_KEXINIT received
debug1: SSH2_MSG_KEXINIT sent
debug1: kex: algorithm: curve25519-sha256@libssh.org
debug1: kex: host key algorithm: ecdsa-sha2-nistp256
debug1: kex: server->client cipher: chacha20-poly1305@openssh.com MAC: <implicit> compression: none
debug1: kex: client->server cipher: chacha20-poly1305@openssh.com MAC: <implicit> compression: none
debug1: expecting SSH2_MSG_KEX_ECDH_REPLY
debug1: rekeying in progress
debug1: rekeying in progress
debug1: Server host key: ecdsa-sha2-nistp256 SHA256:XR7rAZ7Nc73FWhhI15ezsYftiyM0+QUza17v3ExjJtc
debug1: set_newkeys: rekeying, input 3221650236 bytes 134203405 blocks, output 1183488 bytes 32688 blocks
debug1: rekey after 134217728 blocks
debug1: SSH2_MSG_NEWKEYS sent
debug1: expecting SSH2_MSG_NEWKEYS
debug1: SSH2_MSG_NEWKEYS received
debug1: set_newkeys: rekeying, input 3221650248 bytes 134203406 blocks, output 1183488 bytes 0 blocks
debug1: rekey after 134217728 blocks
debug1: SSH2_MSG_KEXINIT received
debug1: SSH2_MSG_KEXINIT sent
debug1: kex: algorithm: curve25519-sha256@libssh.org
debug1: kex: host key algorithm: ecdsa-sha2-nistp256
debug1: kex: server->client cipher: chacha20-poly1305@openssh.com MAC: <implicit> compression: none
debug1: kex: client->server cipher: chacha20-poly1305@openssh.com MAC: <implicit> compression: none
debug1: expecting SSH2_MSG_KEX_ECDH_REPLY
debug1: rekeying in progress
debug1: rekeying in progress
debug1: Server host key: ecdsa-sha2-nistp256 SHA256:XR7rAZ7Nc73FWhhI15ezsYftiyM0+QUza17v3ExjJtc
debug1: set_newkeys: rekeying, input 4295529612 bytes 134202187 blocks, output 1493012 bytes 31234 blocks
debug1: rekey after 134217728 blocks
debug1: SSH2_MSG_NEWKEYS sent
debug1: expecting SSH2_MSG_NEWKEYS
debug1: SSH2_MSG_NEWKEYS received
debug1: set_newkeys: rekeying, input 4295529624 bytes 134202188 blocks, output 1493012 bytes 0 blocks
debug1: rekey after 134217728 blocks
...


^CApplication is shutting down...

//===
$ electronize start
