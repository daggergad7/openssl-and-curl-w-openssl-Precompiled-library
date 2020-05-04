# openSSL and CUrl (w/ openSSL) Precompiled library

in C/C++ -> General -> Additional Include Directories add:

C:\openssl-build\Lib\x32\Release\include;C:\curl-7.69.0-openssl-builds\libcurl-vc16-x86-release-static-ssl-static-ipv6-sspi\include;C:\curl-7.69.0-openssl-builds\libcurl-vc16-x86-release-static-ssl-static-ipv6-sspi\include\curl;%(AdditionalIncludeDirectories)

in Linker -> Input -> Additional Dependencies add:
Normaliz.lib;Ws2_32.lib;Wldap32.lib;Crypt32.lib;advapi32.lib;C:\curl-7.69.0-openssl-builds\libcurl-vc16-x86-release-static-ssl-static-ipv6-sspi\lib\libcurl_a.lib;C:\openssl-build\Lib\x32\Release\lib\libcrypto.lib;C:\openssl-build\Lib\x32\Release\lib\libssl.lib
