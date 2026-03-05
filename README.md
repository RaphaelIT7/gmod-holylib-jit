# HolyLib's custom LuaJIT version
HolyLib has some LuaJIT changes.<br>
These were previously inside the https://github.com/RaphaelIT7/gmod-lua-shared though we moved them here since we should have never done them over there in the first place.<br>

Included changes:
\- [+] Added the ability to concat bool values.<br>
\- [+] Added block debug functionality for function to prevent someone from getting functions they shouldn't have.<br>
\- [+] Added read only table functionality to prevent someone from modifying a table while its being used by another thread<br>
\- [+] Implemented fix for FFI Sandwich/LUA VM re-entry through JIT trace (See https://github.com/LuaJIT/LuaJIT/pull/1165)<br>
\- [+] Experimentally implemented `Sink optimization` (See https://github.com/LuaJIT/LuaJIT/pull/652)<br>
\- [+] Specialize to the global environment change (See https://github.com/LuaJIT/LuaJIT/pull/910)<br>
\- [+] Compile unpack() given constant start and end indices (See https://github.com/LuaJIT/LuaJIT/pull/910)<br>
\- [+] Experimentally implemented `Reduce method overhead in loops by specializing to metatables` (See https://github.com/LuaJIT/LuaJIT/pull/899)<br>
