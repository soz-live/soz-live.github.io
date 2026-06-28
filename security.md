---
layout: default
---

# Security

The safety and security of the code is paramount to develop trust between the developers and the Users and Coders.


## Risks

The running of any code carries with it a certain level of risk, especially from unknown or untrusted sources.  
These risks include:

- Unsecured source code - open to modification by others.
- Code that accesses the computer's registry.
- Code that runs external commands, such as shell or Powershell.
- Code that reads and writes to external files without checking for permission.
- Code that generates side effects as it runs.

### Unsecured Code

**SOZ-LIVE** source code is secured as it:

- is stored in GitHub private repos with only releases made public.
- utilises GitHub tagging and immutable signed releases.
- provides all code in a single Lisp file that the user can access and read through to confirm its safety and suitability for use.
- provides a SHA256 checksum of the file to confirm that no tampering of the file has occurred.

### Registry Access

**SOZ-LIVE** code does not access the registry - all changes are made within the drawing file.

### External Commands

**SOZ-LIVE** code does not run external scripts and commands.

### External Files

**SOZ-LIVE** code only interacts with external files:

- when reading and writing DCL files to build Dialog Boxes on the fly.
- when directed by the user.
- using standard file dialogs.
- in DWG files or human readable text file formats (DAT and CSV) that can be checked by the user.
- doesn't write to external log files.

### Side Effects

**SOZ-LIVE** code doesn't generate side-effects during running as it utilises save and restore methods for the current working state of the drawing inside of commands.

## Dos and Do Nots

- **Do**: only download the releases from the **soz-releases** repo.
- **Do**: check the SHA256 checksum for the downloaded file.
- **Do**: read through the code if possible.
- **Do**: test it first before using it in production.
- **Do Not**: import files (DAT or CSV) without reading them first.
- **Do Not**: load additional code without checking it first.

## Safety

Stay safe, be aware of the potential hazards and be cautious.

For any questions regarding the project please email tim AT soz-live DOT com