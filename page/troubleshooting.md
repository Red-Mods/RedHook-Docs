# 🧰 Troubleshooting

Below you will find a list of the common issues you can encounter when installing or using **RedHook**.

## I'm getting _"Access Violation"_ error at game launch

If you experience access violation errors, please disable software that may conflict with **RedHook**, such as **MSI Afterburner** and **RivaTuner**.

## RedHook/Red Trainer not even loading

Be sure you have installed the latest [Visual C++ Redistributable](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-160) from **Microsoft**. Choose the **x64** version.

![Microsoft Visual C++ Redistributable](https://raw.githubusercontent.com/Red-Mods/RedHook-Docs/main/assets/microsoft_vcpp_link.jpg)

## RedHook is detected as a virus

Some antivirus software may flag **RedHook** as a potential virus. If you encounter this issue, please add an exclusion to your RDR install folder in your antivirus settings. Alternatively, temporarily disable your antivirus software.

## RedHook is partially working but i don't have any visual/doesn't render anything

This is a rare known issue, seems like it's happening only with really old and low end graphics card. You can try to enable VMT hooking in **RedHook.ini** config file.

Go at line:

`UseVMT=false`

and set it to true instead:

`UseVMT=true`