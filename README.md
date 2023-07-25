# BetterPipename
Example of using `Sleep`, and `Java` bindings to create better named pipes.

---
### Problem Statement

As evidenced by modern threat hunting efforts and security products, named pipes and their parent processes are more heavily scrutinized.

---
### Goals
* Provide a "framework" for adding known named pipe nomenclature easily and reliably
* Provide an example of using `Sleep` and its bindings to `Java` to provide a "batteries included" reference
* Supersede the necessity of `Malleable C2` definitions for named pipe nomenclature masks
* Automate, where possible, the ability to create named pipe listeners within `Cobalt Strike`, in a native fashion
* Prevent the possibility of name collision
* Remove the ability of operator-introduced errors

---
### How to Use
- Load the `pipename.cna` file into the `Cobalt Strike` `Script Manager`
- From the context of any selected `Beacon`:
  - Right click, selecting `Generate SMB Pipe Listener`
  - Select the desired `Pipe Type` from the dropdown menu:
    - `chrome_mojo`
    - `chrome_sync`
    - `crashpad`
    - `dotnet`
    - `powershell`
    - `powershell_ise`
  - Select `Generate`
  - Your respective and appropriately-named `SMB` pipe listener will be found in the `Listeners` menu within the `Cobalt Strike` UI

---
### References and Credits

- [Austin Hudson](https://twitter.com/ilove2pwn_)
- [Falcon Force Friday](https://medium.com/falconforce/falconfriday-suspicious-named-pipe-events-0xff1b-fe475d7ebd8)
