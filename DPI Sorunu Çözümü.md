
MANIFEST DOSYASI FARK KARŞILAŞTIRMASI (DPI DÜZENLEMESİ)
=======================================================

Aşağıda, orijinal app.manifest dosyan ile DPI destekli sürüm arasındaki farkları görebilirsin.

Açıklama:
- YEŞİL 🟢 satırlar: Eklenen yeni ayarlar
- KIRMIZI 🔴 satırlar: Silinen veya yoruma alınan satırlar
- Normal satırlar: Değişmeyen bölümler

-------------------------------------------------------

<?xml version="1.0" encoding="utf-8"?>
<assembly manifestVersion="1.0" xmlns="urn:schemas-microsoft-com:asm.v1">
  <assemblyIdentity version="1.0.0.0" name="MyApplication.app"/>
  <trustInfo xmlns="urn:schemas-microsoft-com:asm.v2">
    <security>
      <requestedPrivileges xmlns="urn:schemas-microsoft-com:asm.v3">
        <requestedExecutionLevel level="asInvoker" uiAccess="false" />
      </requestedPrivileges>
    </security>
  </trustInfo>

  <compatibility xmlns="urn:schemas-microsoft-com:compatibility.v1">
    <application>
🔴   <!--<supportedOS Id="{e2011457-1546-43c5-a5fe-008deee3d3f0}" />--> <!-- Windows Vista -->
🔴   <!--<supportedOS Id="{35138b9a-5d96-4fbd-8e2d-a2440225f93a}" />--> <!-- Windows 7 -->
🔴   <!--<supportedOS Id="{4a2f28e3-53b9-4441-ba9c-d69d4a4a6e38}" />--> <!-- Windows 8 -->
🔴   <!--<supportedOS Id="{1f676c76-80e1-4239-95bb-83d0f6d0da78}" />--> <!-- Windows 8.1 -->
🔴   <!--<supportedOS Id="{8e0f7a12-bfb3-4fe8-b9a5-48fd50a15a9a}" />--> <!-- Windows 10 -->
🟢     <supportedOS Id="{8e0f7a12-bfb3-4fe8-b9a5-48fd50a15a9a}" /> <!-- Windows 10 -->
🟢     <supportedOS Id="{4f476546-0e43-4a99-9c6d-f47d961dfb5b}" /> <!-- Windows 11 -->
    </application>
  </compatibility>

🟢 <application xmlns="urn:schemas-microsoft-com:asm.v3">
🟢   <windowsSettings>
🟢     <dpiAware xmlns="http://schemas.microsoft.com/SMI/2005/WindowsSettings">true/pm</dpiAware>
🟢     <longPathAware xmlns="http://schemas.microsoft.com/SMI/2016/WindowsSettings">true</longPathAware>
🟢   </windowsSettings>
🟢 </application>

🔴   <!--<application xmlns="urn:schemas-microsoft-com:asm.v3">
🔴     <windowsSettings>
🔴       <dpiAware xmlns="http://schemas.microsoft.com/SMI/2005/WindowsSettings">true</dpiAware>
🔴       <longPathAware xmlns="http://schemas.microsoft.com/SMI/2016/WindowsSettings">true</longPathAware>
🔴     </windowsSettings>
🔴   </application>-->

🔴   <!--<dependency>
🔴     <dependentAssembly>
🔴       <assemblyIdentity
🔴           type="win32"
🔴           name="Microsoft.Windows.Common-Controls"
🔴           version="6.0.0.0"
🔴           processorArchitecture="*"
🔴           publicKeyToken="6595b64144ccf1df"
🔴           language="*"
🔴         />
🔴     </dependentAssembly>
🔴   </dependency>-->

</assembly>
