# Windows-Registry-Tools
Tools for adding, changing, removing in Windows Registry 

## EnableCommonNameFallbackForLocalAnchors (May 24, 2017)

* To Enable setting opens Enable-EnableCommonNameFallbackForLocalAnchors.reg.
* To Remove setting opens Disable-EnableCommonNameFallbackForLocalAnchors.reg.

The tool is for using Google Chrome 58 or above version with Symantec product. 

### How to do the setting manually

1. Open Registry editor on your Windows.
2. Added the following key and value in HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Google\Chrome  
key = EnableCommonNameFallbackForLocalAnchors  
value = 00000001  
type = dword  

### Reference

* NET::ERR_CERT_COMMON_NAME_INVALID when using HTTPS inspection (https://support.symantec.com/en_US/article.TECH240507.html)
* Chrome no longer accepts certificates that fallback to common name (ERR_CERT_COMMON_NAME_INVALID)	 (https://bugs.chromium.org/p/chromium/issues/detail?id=700595&desc=2)

