# HolyLib's custom LuaJIT version
HolyLib has some LuaJIT changes.<br>
These were previously inside the https://github.com/RaphaelIT7/gmod-lua-shared though we moved them here since we should have never done them over there in the first place.<br>

Included changes:
\- [+] Implemented fix for FFI Sandwich/LUA VM re-entry through JIT trace (See https://github.com/LuaJIT/LuaJIT/pull/1165)<br>
\- [+] Experimentally implemented `Sink optimization` (See https://github.com/LuaJIT/LuaJIT/pull/652)<br>
