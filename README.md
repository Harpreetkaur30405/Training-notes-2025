# 25/06/2025
## Linux over Windows
### Why to use Linux over Windows?


| Reason                         | Explanation
| ------------------------------ | ------------------------------------------------------------------------------- |
| **Cost**                       | Linux is free, while windows requires a paid license.                           |
| **Open Source**                | Linux's code is open for review, customization, and improvement.                |
| **Security**                   | Linux requires host password for every change hence it's more secure.           |
| **Customizability**            | Linux offers extensive options to customize the UI.                             |
| **Performance**                | Linux can run efficiently on older hardware.                                    |
| **Software Freedom**           | You can freely modify and redistribute Linux software.                          |
| **Stability and Reliability**  | Preferred over servers and critical systems due to strong stability.            |
| **Community Support**          | Large, active communities for help and troubleshooting.                         |
| **No Forced Updates**          | Users control when and what updates to install. It's never "take it or leave it", there's always choices. |


### Downloaded 3 softwares:
1. [Oracle Virtual Machine](https://download.virtualbox.org/virtualbox/7.0.20/VirtualBox-7.0.20-163906-Win.exe)
2. [Ubuntu 24.04.02](https://login.gndec.ac.in/ubuntu-24.04.2-desktop-amd64.iso)
3. [Microsoft Visual C++](https://download.visualstudio.microsoft.com/download/pr/40b59c73-1480-4caf-ab5b-4886f176bf71/D62841375B90782B1829483AC75695CCEF680A8F13E7DE569B992EF33C6CD14A/VC_redist.x64.exe)


**After installation, start Oracle VM.**
- Go to new.
- Then enter the name, *Ubuntu*.
- Select the path of Ubuntu in ISO image.
- Enter password and username.
- Give required memory space and Processors.
## Issues faced:
After powering up, the display only showed a black screen with error:

-  ![Error image](error.jpg)
+  ![error image](https://github.com/user-attachments/assets/4fd4979a-2e93-4d00-af05-fbb406bb9172)

**To solve:**
- Go to settings -> Display
- Change the Graphics Controller to **VBoxVGA.**
 
-   ![Resolved image](resolved.jpg)
+   ![Resolved image](https://github.com/user-attachments/assets/3738fb23-6442-4cf1-86f9-040ed2715919)

## Booting and its types:
Booting is the process of starting up or restarting a computer, which involves initializing hardware, loading the <br> operating system, and preparing the computer for use.
### Types of Booting:
- **Cold boot/ Hard boot:**
  This refers to starting the computer from a completely powered-off state.
- **Warm boot/ Soft boot:**
  This is when the operating system alone is restarted without turning it off.

# 26/06/2025

## Introduction to Linux Shell and basic commands:
### Kernel:
- The kernel is a computer program that is the core of a computer's operating system, with complete control over everything in the system.
- Think of it as chef working in a hotel. You as a customer can't see the chef working but get your order (output).

  ### Shell:
  - Shell is a special user program that provides an interface for the user to use operating system services.
  - Using the same scenario, think of shell as a waiter, who takes your order (input) and gives it to the chef (Kernel).
 
  Shell is divided into two categories:
 + 1. Command Line Shell:


     ![Command line shell](https://github.com/user-attachments/assets/326374f1-95f8-4508-b9cb-2167573778ab)
+    
  2. Graphical Shell:

    ![Graphical shell](https://github.com/user-attachments/assets/fbc1d0d0-80e9-41fd-8a61-1c3c99dd9f02)


  **Types of shell:**
  - BASH (Bourne Again Shell)
  - CSH (C Shell)
  - KSH (Korn Shell)

   ### File system structure:
   |NAME        | DESCRIPTION                                                                             |
   | ---------- | --------------------------------------------------------------------------------------- |
   | `/`        | The slash / character denotes the root of the filesystem tree. exp: Trunck of a tree.|
   | `/home`    | Contains personal directories of user.|
   | `/lib`     | Contains system libraries and critical file.|
   | `/bin`     | Contains user executable files.|
   | `/boot`    | Contains all the files that are required for booting.|
   | `/dev`     | Contains hardware and development files.|
   | `/media`   | Mount points for removable media.|
   | `/mnt`     | Temporarily mounted file systems.|
   | `/opt`     | Contains optional files.|

   ## Commands:
-  - `ls` (list): Returns content of a specified Directory.
-  - `whoami`: Returns the current domain and user name.
   - `date`: Returns current date.
-  - `pwd`: Prints the current working directory.
-  - `mkdir`: Creates a new directory.
+  - `whoami`: Returns the current domain and user name.
+  - `ls` (list): Returns content of a specified Directory.
   - `cd`: Changes directory

  ![date_whoami_ls_cd](https://github.com/user-attachments/assets/cb285b22-6cfb-4caa-9fdf-3c94b923f426)

+  - `mkdir`: Creates a new directory.
+  - `pwd`: Prints the current working directory.

   ![mkdir_pwd](https://github.com/user-attachments/assets/321f1ea0-628b-421b-9f15-b450f469d149)


   - `touch`: Creates empty file.
   - `cat`: Creates file with content.

  ![cat_touch](https://github.com/user-attachments/assets/2ad1ef93-d725-4075-beca-f6b68b7c3acf)

   - `whereis`: Finds the loxcation of specified files.
-  `whatis`: Gives short description of a command.

     ![whereis](https://github.com/user-attachments/assets/aa2b8347-fafe-4947-b723-c7604157334e)

   -  `mv`: To move or rename a file.

      ![mv](https://github.com/user-attachments/assets/c6d6bf2e-b6f5-4938-adf8-f605f8840737)

   -   `cp`: To copy content of a file to the other.

       ![cp](https://github.com/user-attachments/assets/b43ca138-15df-4daa-b1b8-414da5bda378)

+  -   `whatis`: Give short description of a command.
     
+  ## Issues faced:
+  Running `whatis command` always returns "nothing appropriate"

  ![whatis_error](https://github.com/user-attachments/assets/5b60bf43-cb7d-49e5-880b-1347b12814d8)
  
+  **Solution found:**
+  `whatis` uses an index created and maintained by `mandb` to locate the documentation you're looking for. If said index doesn't exist, or if the command you're looking for isn't in the existing index, you'll see Nothing appropriate. If your setup doesn't have a `mandb` index yet, you can create one by running `sudo mandb`.

   ![whatis_solved](https://github.com/user-attachments/assets/be581476-fc20-4291-9885-02d620903830)
  ## Introduction to Linux Shell and basic commands:
### Kernel:
- The kernel is a computer program that is the core of a computer's operating system, with complete control over everything in the system.
- Think of it as chef working in a hotel. You as a customer can't see the chef working but get your order (output).

  ### Shell:
  - Shell is a special user program that provides an interface for the user to use operating system services.
  - Using the same scenario, think of shell as a waiter, who takes your order (input) and gives it to the chef (Kernel).
 
  Shell is divided into two categories:
 + 1. Command Line Shell:


     ![Command line shell](https://github.com/user-attachments/assets/326374f1-95f8-4508-b9cb-2167573778ab)
+    
  2. Graphical Shell:

    ![Graphical shell](https://github.com/user-attachments/assets/fbc1d0d0-80e9-41fd-8a61-1c3c99dd9f02)


  **Types of shell:**
  - BASH (Bourne Again Shell)
  - CSH (C Shell)
  - KSH (Korn Shell)

   ### File system structure:
   |NAME        | DESCRIPTION                                                                             |
   | ---------- | --------------------------------------------------------------------------------------- |
   | `/`        | The slash / character denotes the root of the filesystem tree. exp: Trunck of a tree.|
   | `/home`    | Contains personal directories of user.|
   | `/lib`     | Contains system libraries and critical file.|
   | `/bin`     | Contains user executable files.|
   | `/boot`    | Contains all the files that are required for booting.|
   | `/dev`     | Contains hardware and development files.|
   | `/media`   | Mount points for removable media.|
   | `/mnt`     | Temporarily mounted file systems.|
   | `/opt`     | Contains optional files.|

   ## Commands:
-  - `ls` (list): Returns content of a specified Directory.
-  - `whoami`: Returns the current domain and user name.
   - `date`: Returns current date.
-  - `pwd`: Prints the current working directory.
-  - `mkdir`: Creates a new directory.
+  - `whoami`: Returns the current domain and user name.
+  - `ls` (list): Returns content of a specified Directory.
   - `cd`: Changes directory

  ![date_whoami_ls_cd](https://github.com/user-attachments/assets/cb285b22-6cfb-4caa-9fdf-3c94b923f426)

+  - `mkdir`: Creates a new directory.
+  - `pwd`: Prints the current working directory.

   ![mkdir_pwd](https://github.com/user-attachments/assets/321f1ea0-628b-421b-9f15-b450f469d149)


   - `touch`: Creates empty file.
   - `cat`: Creates file with content.

  ![cat_touch](https://github.com/user-attachments/assets/2ad1ef93-d725-4075-beca-f6b68b7c3acf)

   - `whereis`: Finds the loxcation of specified files.
-  `whatis`: Gives short description of a command.

     ![whereis](https://github.com/user-attachments/assets/aa2b8347-fafe-4947-b723-c7604157334e)

   -  `mv`: To move or rename a file.

      ![mv](https://github.com/user-attachments/assets/c6d6bf2e-b6f5-4938-adf8-f605f8840737)

   -   `cp`: To copy content of a file to the other.

       ![cp](https://github.com/user-attachments/assets/b43ca138-15df-4daa-b1b8-414da5bda378)

+  -   `whatis`: Give short description of a command.
     
+  ## Issues faced:
+  Running `whatis command` always returns "nothing appropriate"

  ![whatis_error](https://github.com/user-attachments/assets/5b60bf43-cb7d-49e5-880b-1347b12814d8)
  
+  **Solution found:**
+  `whatis` uses an index created and maintained by `mandb` to locate the documentation you're looking for. If said index doesn't exist, or if the command you're looking for isn't in the existing index, you'll see Nothing appropriate. If your setup doesn't have a `mandb` index yet, you can create one by running `sudo mandb`.

   ![whatis_solved](https://github.com/user-attachments/assets/be581476-fc20-4291-9885-02d620903830)

   # 27/06/2025

   ## Permissions & Shell programming:
### File and directory permissions:
`chmod` (Change mode): It is used to change the access permissions of files and directories.

Some differenet chmod permisssion notations are:<br>
  `chmod` +x test.sh: Gives permission to run the script.<br>
  `chmod` 444 test.sh: Changes file to read-only

![read only](https://github.com/user-attachments/assets/f335b301-8398-4e7b-b4b8-da9ab4fadcdb)

*Result* <br>
![read-only_result](https://github.com/user-attachments/assets/42e27596-e10e-4f6a-bdb4-40513b6e9d20)


  `chmod 644 test.sh`: Changes file such that only owner can edit it. For others it remain read-only.

![user_writable](https://github.com/user-attachments/assets/c950b20e-34b1-48ce-8222-52ac5b304557)

*Result* <br>
![user-writable_result](https://github.com/user-attachments/assets/524f435f-3f3c-43cb-9826-37d1ef8e7d95)

 `chown` (Change Owner): It is a command used to change the ownership of files or directories to a different user or group. 
 
 `To change owner`: 

![Change owner](https://github.com/user-attachments/assets/939eac1d-5f2c-4601-acf9-556032d7c701)

 `To change group`:

 ![Change group](https://github.com/user-attachments/assets/1d35ebc8-8935-4a78-93c1-c19e023a5920)

Grep: It is a command to search for specific text or patterns within files or command output.

![grep](https://github.com/user-attachments/assets/b05457f5-dccc-434b-9e72-529b6c025002)

### Shell Programming:
1. Use of variables:

![variables](https://github.com/user-attachments/assets/ecf1bd9c-a252-4e15-b76c-69662508a78f)

*Output* <br>
![variables result](https://github.com/user-attachments/assets/e8115fd1-72b9-41b2-b7ef-de196ca4b048)


2. Comparing Two numbers

![Compare numbers](https://github.com/user-attachments/assets/38a51327-c40e-42ae-b125-ec6a4cb0c555)

*Output* <br>
![Test result](https://github.com/user-attachments/assets/1b46a995-a01e-4655-b61f-0ee956de3fe3)



## Other short topics:
### Partitioning Scheme:


A **partitioning scheme**is the way a hard disk or SSD is **divided into sections** (partitions) so the system can use it properly.

**It is used for:**<br>
* Sepaerate **system files** from **user files**
* Install **multiple OSes**
* Create **swap space**
* Improve **backup & security**


### Types of Partitioning Scheme:

#### 1. MBR (Master Boot record):
- Max 4 primary partitions.
- Supports up to 2 TB.
- Older, used with BIOS.
- less flexible

#### 2. **GPT (guided Partition table)**
- Supports 128+ partitions.
- Works with disks >2 TB.
- Newer, used with UEFI.
- more flexible

### Bare Metal Installation:

* Installation directly using USB.
* Direct installation in computer hardware.
* No OS should be in between.

### Redirection:
It allows user to redirect input and output functionalities to the files or folders.

**Types of Redirection:**
1. Overwrite Redirection (For stdout):<br>
Redirects the standard output of a command to a file. If the file exists already contain script, it will be overwritten. ">" standard output


2. Append Redirection (For stdout):
Append the output to the file without compromising the existing data of the file.


3. Overwrite Redirection (For stdin):<br>
Redirects the standard input of a command to a file. "<" standard input


### Pipe '|':
The pipe is used to combine two or more commands, and in this, the output of one command acts as input to another command.
- Pipe can be used for filteration.
- Multiple pipes can be used such as:
  To find number of file/directory with 't'.

### Wild cards:

| Wildcard | Meaning                              |
| -------- | ------------------------------------ |
| `*`      | Matches **zero or more** characters  |
| `?`      | Matches **exactly one** character    |
| `[abc]`  | Matches **one character** from set   |

### File Compression:
File compression reduces file size to save space or speed up transfer.
- `gzip`:
  - Used to zip a file.
  - Limitation: The original file is deleted.
- `gunzip`:
  - Unzips the file.
-  Flag `-k`:
   - To zip the file
   - Original file isn't deleted. 

# 30/06/2025

## PC Hardware Troubleshooting:
### Components of CPU:
### 1. Motherboard:
A motherboard is the main circuit board in a computer system. It connects all of the internal components, like the memory, processor, graphics card and other hadrware. Its also known as PCB (Printed circuit board).

*Some componeents of Motherboard:* <br>
- **Processor Socket:** <br>
  It is mechanical and electrical interface on a motherboard that securely connects a central processing unit (CPU) to the rest of the computer system.

- **CMOS backup battery:** <br>
  It is a small, coin-shaped battery that helps to keep the date and time accurate on computer. It ensures these settings are retained even when the computer is turned off and disconnected from a power source.

- **LAN (Local area network):** <br>
  It is the built-in Ethernet port that allows the conmputer to connect to a wired local area network for internet and data communication.

- **RAM Slots:** <br>
  Slots for installing RAM (Random Access Memory) modules.

- **Chipset:** <br>
  Communication between Northbridge (handles CPU, RAM, GPU communication) and Southbridge (handles I/O, storage decvices).

- **Expansion Slots:** <br>
  - Expansion slots on a motherboard are sockets designed to accomodate expansion cards, which add or enhance a computer's functionality.
  - Common types: PCI

- **Power Connectors:** <br>
  Connects to the power supply unit (PSU).

- **Storage Connectors:** <br>
  SATA ports for connecting hard Drives (HDD), Solid-State Drives (SSD), and Optical Drives.

- **BIOS Chip:** <br>
  Firmware that initializes hardware during startup and provides runtime services for the OS.

- **Input/Output (I/O) Ports:** <br>
  - Located on the back of the motherboard.
  - Includes USB ports, audio jacks, Ethernet, HDMI, DisplayPort, PS/2, etc.

- **Heat Sinks:** <br>
  passive cooling components for chipsets and VRMs.

![components-of-motherboard](https://github.com/user-attachments/assets/350d1dd5-62c7-4c8c-964c-65aeb110688c)

### 2. **Fan:**

* Used for cooling the motherboard.
* Prevents overheating.

### 3. **Power Supply with Fan**

 * Provides **electrical power** to all parts of the computer.
 * Has a **built-in-fan** to cool itself & CPU cabinet during operation.
 * Converts electricity from the wall (AC) to usable computer power (DC).

### 4. **Connectors**

* Cables and plugs that connect components to the power supply and motherboard.

### 5. **Expansion Slots**
* Used to insert extra cards like:<br>
  * **Graphics cards**
  * **Sound cards**
  * **Wi-Fi/network cards**

### 6. **Hard Disk Drive (HDD):**
* Stores data, software, and the operating system.
* Located **under the optical drive** in the cabinet.

### 7. **Optical Drive (CD/DVD Drive):**

* Used to read/write **CDs and DVDs**

*How to locate components of a CPU?*

- Look for the power supply with fan (usually at the back top or bottom of the cabinet).
- In front of it is the optical drive.
- On it's side is the Motherboard.
- Below the optical drive is the hard disk drive. 

### Difference between RAM and cache memory:

|Feature         | **RAM (Random Access Memory)**                                      | **Cache Memory**                          |
| -------------- | ------------------------------------------------------------------- | ----------------------------------------- |
| **Purpose**    | It holds programs and data that are currently executed by the CPU.  | It holds frequently used data by the CPU. |
| **Speed**      | Slower than cache                                                   | Much faster than RAM                      |
| **Size**       | Larger (in GBs, e.g., 8GB, 16GB)                                    | Smaller than RAM                          |

**Why do we need Cache memory?**
- It helps the **CPU work faster and more efficiently** by reducing the time it takes to access data.
  * Cache memory is **musch faster** than RAM.
  * It stores **frequently used instructions and data**, so the CPU doesn't have to wait for slower RAM.
  * Without cache, the Processor would **waste cycles**.<br>
So it is used to remove mismatch between RAM and Processor speed.

### Difference between RAM and Hard Disk:
| Feature                | RAM (Random Access Memory                       | Hard Disk                                     |
| ---------------------- | ----------------------------------------------- | --------------------------------------------- |
| **Purpose**            | Temporary memory for currently running programs | Permanent storage for files, software and OS  |
| **Storage type**       | Temporary (loses data when off)                 | Permanent (Keeps data when off)               |
| **Speed**              | Much faster                                     | Slower compared to RAM                        |
| **Storage Capacity**   | Smaller                                         | Larger                                        |
| **Access Method**      | Direct access by CPU                            | Slower access through file system             |
| **Cost**               | Expensive                                       | Cheaper                                       |
| **Function**           | Helps run active programs and processes         | Stores data, files, OS and installed programs |

**Process of Booting:**                            
| **Step**                                        | **Description**                                                      |
| ----------------------------------------------- | -------------------------------------------------------------------- |
| **1. Power On**                                 | You press the **power button**. Electricity flows to all components. |
| **2. Signal to RAM (Firmware loads bootstrap)** | The **BIOS/UEFI firmware** stored in ROM sends a signal to RAM and loads Bootstrap Loader. |
| **3. Hard Disk Copy Transferred to RAM**        | The Bootstrap Loader finds the operating system (OS) on the hard disk and copies essential OS files into RAM. |
| **4. OS Starts (OS gets control)**              | Once the OS is loaded into RAM, it takes over the system. The desktop/interface appears, and the system is ready for use.|

## Basic boot Issues:
*1. No Power*
 - Computer does not turn on at all.
 - No lights, no fan noise, screen remains black.
 - Cause: Faulty power supply, loose cables, dead battery

*2. No Display / Black Screen*
 - Computer powers on, but nothing shows on screen

*3. Beep Codes*
 - System gives beep sounds indicating hardware errors (RAM, CPU)

*4. POST Failure*
 - Power-On Self-test fails; system may freeze or beep

*5. Blue Screen of Death (BSOD)*
 - Windows crashes with a blue screen error

## Common issues and problems in PC:

### GPU (Graphics processor unit):
- Responsible for rendering graphics and visual output.
- Problems include overheating, driver issues, screen tearing, or no display output.

### PCU (Personal Computer Unit):
1. Installation and Hard Disk Preparation:<br>

* Partitioning: the first step of partitioning is to organize the hard disk into:
  * **Primary (C: Drive):** <br>
    - Where the Operating System (Windows/Linux/Unix) is installed.
    - Avoid storing personal/important files in **C:**
    - If Windows crashes, files in D:, E:, F: are safer and can often be recovered.
* **Logical Drives (D:, E:, F:):** used for pictures, videos, documents, etc.

2. Speed slow (Causes & Fixes): 
-       Desktop:
        Files should be on drive. By default files on desktop are stored on C drive.
        As Os system is installed in C: file, its recommend to put many folders in desktop.
        Move them into drives.

-       Task Bar:
        keep minimal shortcuts on the taskbar.

-       Browser (Bookmarks):
        Avoid excessive browser bookmarks as they slow down browser start-up.

-       Temporary files:
        These files are created by websites & cookies, and stored/ download in hidden files.
        Ultimately because of it the system slows down. So, after a period of time remove temporary files.

-       RAM overuse:
        Don't open a number of applications or tabs are open at once. As ultimately we are using the RAM.

-       Malware:
        Regularly scan your system for malwares.

-       Fragmentation: 
        There shouldn't be chaos or dely to access files. <br>
        To make system efficient in working and get work done in optimal way, defragmentation is done. 
        * Go to start -> Defragment and Optimize drives
        * Schedule defragmentation for automatic optimization.

3. Printer Issues & solutions:

| Problem                                 | Solution                                    |
| --------------------------------------- | ------------------------------------------- |
| Paper Jam                               | Remove the stuck page carefully             |
| Printer Out of Paper During Print Job   | Use Queue                                   |
| Faded or Poor Quality Prints            | Refill or replace ink/toner                 |
| Overlapping Lines in print              | Possible **drum issue**, replace the drum   |

### Blue Screen of Death (BSOD):
It is used to indicate a system crash, in which the operating system reaches a critical condition where it can no longer operate safely.

**Common Causes of BSOD:**

1. Hardware Failures: <br>
   faulty RAM<, hard disk, or other internal components
2. Driver Issues: <br>
   Outdated, incompatible, or corrupted device drivers
3. Corrupted System Files: <br>
   System file corruption due to improper shutdowns, malware, or failed updates
4. Overheating or Power issues: <br>
   Inadequate cooling or power supply malfunctions

# 01/07/2025

## System Crash Analysis:

After a BSOD, Windows creates a **dump file** that records what happened before the crash.

### Tools for Analysis:
1. **event Viewer:** <br>
   Windows tool to check detailed system and crash logs.
2. **WinDbg:** <br>
   Microsoft Debugging Tool for analyzing dump files.

### BIOS/UEFI Settings and POST Errors:

| BIOS                       | UEFI                                   |
| -------------------------- | -------------------------------------- |
| Basic Input/Output System  | Unified Extensible Firmware Interface  |
| Older firmware standard    | Modern replacement for BIOS            |
| Keyboard-only navigation   | Supports mouse and GUI                 |
| Stored in ROM chip         | stored in flash memory                 |

BIOS/UEFI is responsible for initializing hardware components before the OS loads.


**What is POST?:** <br>
POST (Power-On Self Test) is a diagnostic process that occurs when the computer is powered on. It checks for:

* RAM functionality
* CPU status
* Keyboard presence
* Display detection
* Hard disk and drives

*Common POST Errors:*

| Beep Code / Mesaage    | Meaning                                                     |
| ---------------------- | ----------------------------------------------------------- |
| 1 Long, 2 Short beeps  | Graphics card issue                                         |
| Continuous Beeps       | RAM failure                                                 |
| No beep, No Display    | Power or motherboard issue                                  |
| "CMOS Checksum Error"  | Corrupted BIOS settings (usually fixed by resetting CMOS)   |

### Accessing BIOS/UEFI Settings

* Press **F2**, **F10**, **DEL**, or **ESC** continuously during startup (key depends on manufacturer).
* From here, you can:

  * Change boot order
  * Enable/Disable hardware components
  * View system info
  * Reset settings to default (if needed)


---
### Other small concepts:

**Wizard-Based Installation:** <br>
GUI-based installation with no need to type commands.

**Antivirus Installation:** <br>
Essential for protection against viruses, malware, and spyware.

**Help Shortcut:** <br>
Press **F1** to open help tool in Windows.

## IP Address:
An IP address (Internet Protocol address) is a unique numerical label assigned to each drive connected to a computer network that uses the Internet Protocol for communication. It acts as an identifier for the device on the network.

## Command Prompt:
*1. ipconfig:*
   ipconfig is a Command Prompt command used to display and manage the IP address and network settings of a computer in a Windows operating system.

*2. ping:*
    The ping command is used to test the connectivity between your computer and another device or server over a network.

*3. tracert:*
    The tracert (Trace Route) command is used to track the path that data takes from your computer to a destination across a network.

# 02/07/2025

## Safe Mode:
Safe Mode is a diagnostic mode in Windows that starts the computer with a minimal set of drivers and services, which makes it easier to find and remove harmful malware and viruses without activating them.

**Types of Safe Mode:** <br>
1. Safe Mode:<br>
   Used to diagnose and fix basic system issues.

2. Safe Mode with Networking: <br>
   Includes network drivers and services. Allowing access to thew internet or network drives for troubleshooting.

3. Safe Mode with Command Prompt:<br>
   Loads a minimal environment with Command Prompt instead of the normal desktop interface.

## How to make a RJ-45 Cable:
1. Strip the Cable to remove 1 inch of the outer sheat.
2. Untwist and straighten the wires inside of the cable.
3. Arrange the wires into the right order.

| **Pin Number**  | **Wire Color (T568B)**   | **Signal**        |
| --------------- | ------------------------ | ----------------- |
| 1               | White Orange             | Transmit + (TX+)  |
| 2               | Orange                   | Transmit - (TX-)  |
| 3               | White Green              | Receive + (RX+)   |         
| 4               | Blue                     | Unused / PoE +    |
| 5               | White Blue               | Unused / PoE +    |
| 6               | Green                    | Receive - (RX-)   |
| 7               | White Brown              | Unused / PoE -    |
| 8               | Brown                    | Unused / PoE -    |

4. Trim the wires into an even line 1/2 inch (13 mm) from sheathing.
5. Insert the wires into the RJ-45 connector.
6. Stick the connector into the crimping part of the tool and squeeze twice.
7. Remove the cable from the tool and check that all of the pins are down & test the cable.

![RJ45-02](https://github.com/user-attachments/assets/2f81216e-cc40-40ca-826e-a21e30da39f0)

# 03/07/2025

## Viruses:
A computer virus is a malicious software program designed to:
 - Infect your computer without your permission.
 - Spread to other systems (like a biological virus).
 - Damage, steal, or corrupt data and files.
 - Sometimes even slow down or crash your computer.

### *Types of Viruses:*
***1. File infector Virus:***
- **What it does:** Attaches to program or system files (like .exe, .dll).
- **Effect:** Corrupts or delete files, slows system.
- **Example:** When you open an infected file, the virus spreads.

***2. Boot Sector Virus:***
- **What it does:** Infects the boot sector (the part that helps start your computer.)
- **Effect:** Stops system from booting properly.
- **Spread:** Mostly through USB drives or CDs.
- **Example:** Michelangelo virus.

***3. Macro Virus:***
- **What it does:** Targets software like Microsoft Word or Excel using macros (small programs).
- **Effect:** Corrupts documents, spreads through email attachments.
- **Example:** Melissa virus.

***4. Polymorphic Virus:***
- **What it does:** Changes its code every time it runs to avoid detection.
- **Effect:** Hard to detect by antivirus software.
- **Example:** Storm Worm.

***5. Resident Virus:***
- **What it does:** Hides in your system's memory (RAM).
- **Effect:** Infects files when opened, even if the original virus is deleted.
- **Example:** Randex, CMJ.

***6. Multipartite Virus:***
- **What it does:** Spreads in multiple ways - infects files and boot sector both.
- **Effect:** Hard to remove as it affects different areas.
- **Example:** Ghostball

***7. Web Scripting Virus:***
- **What it does:** Attacks through malicious scripts on websites.
- **Effect:** Steal cookies, session data, or redirects you.
- **Spread:** Through unsafe websites or popups.

*How we can protect the computer from viruses?*

To **protect your computer from viruses,** follow these **simple but powerful steps:**

***1. Install Antivirus Software:***
- Use trusted antivirus programs like **Norton, Quick Heal, Avast, Bitdefender,** etc.
- Keep the antivirus **updated regularly.**

***2. Keep Your System Updated:***
- Always update your **Windows or other OS.**
- Updates fix **security holes** that viruses can exploit.

***3. Avoid Downloading from Unknown Sources:***
- Do **NOT download software, movies, games or files** from unsafe websites.
- Only use **official or trusted platforms.**

***4. Be Careful with Email Attachments:**
- Never open **suspicious emails** or attachments from **unknown senders.**
- Phishing emails often carry viruses.

***5. Scan USB Drives and CDs:***
- Always **scan pen drives, CDs/DVDs** before opening their contents.
- Avoid using **public/shared USBs.**

### What is Driver Issues?
A **driver** is a **small software program** that helps your **hardware (like mouse, keyboard, printer, etc.) communicatewith your operating system** (like Windows, Linux). 

### Operating System Repair:
**Operating System (OS) repair** means fixing problems in your computer's operating sytem (like **Windows, Linux, or macOS**) when it is not working properly. 

# 07/07/2025

## **Introduction to HTML & Web Basics**

### HTML:
* HTML stamds for HyperText Markup Language.
* It is the standard markup language for creating web pages and web applications.
* HTML defines the structure and content of a web page.

### **How browsers render it:**

1. The broswer reads the HTMl file line by line.
2. It builds the **DOM (Document Object Model)** - a tree-like structure of the page.
3. The browser then displays the structured content visually based on HTMl + CSS.

### Structure of an HTMl Document
* `<!DOCTYPE>` declaration defines that this document is an HTML document
* `<html>` element is the root element of an HTML page
* `<head>` element contains meta information about the HTML page
* `<title>` element specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab)
* `<body>` element defines the document's body, and is a conatiner for all the visible contents, such as headings, pargraphs, images, hyperlinks, tables, lists, etc.
* `<h1>` element defines a large heading
* `<p>` element defines a paragraph

![html](https://github.com/user-attachments/assets/76abad65-126d-49f2-bd2f-2530dc44795d)

### HTML Links:
HTML links are used to connect one web page to another or to external websites. They are created using the anchor tag and usually appear as clickable text or images.


![link](https://github.com/user-attachments/assets/accdc4ce-8e2d-4c53-b375-fea89188da61)

- Href attribute specifies tyhe link's destination (URl or file).

### HTML Images:
HTML images are used to display pictures on a webpage. The img tag is used to embed an image using the src (source) attribute.

![image source](https://github.com/user-attachments/assets/e8b19fc7-3a80-4df2-902a-ed4972a85ed3)

- src(source): path or URL of the image
- alt (alternative text): text shown if image doesn't load
- width and height: size of the image

### The style attribute:
The style attribute is used to add styles to an element, such as color, font, size, and more.


![style](https://github.com/user-attachments/assets/5a8000dd-7632-4d6f-8d8b-5860392f8575)

### Unorderded list:
An unordered list displays items with bullets. It does not follow any order.

![unordered list](https://github.com/user-attachments/assets/2a04bedc-93cc-49db-b27c-93a65d9db366)

### ordered list:
An ordered list displays items in a numbered (1, 2, 3...) or lettered (A, B, C...) order.

![ordered list](https://github.com/user-attachments/assets/f08777c6-a1cd-4b0b-af63-4099e7f7e53e)

### HTML Div Element:
The div element in HTMl is a container used to group other HTMl elements together. It is commonly used for layout, styling, and organizing content using CSS or JavaScript.

![div element](https://github.com/user-attachments/assets/fc429339-add1-4f48-bfa9-c4462d28f395)

# 08/07/2025

## The ID Attribute:
The id attribute in HTML is used to assign a unique identifier to an element. It helps to style, acccess, or link that specific element using CSS, javaScript, or anchor links.

![id](https://github.com/user-attachments/assets/31233807-4d14-4ebe-855f-d31e48f9f453)

## The Class Attribute:
The class attribute in HTML is used to group elements together by assigning them a common name, so they can be styled or accessed collectively using CSS or JavaScript. 

![class](https://github.com/user-attachments/assets/7509e430-c407-4e3c-bcdb-b82b1e93864b)

## Padding:
Padding is the space between the content of an element of an element and its border. It is used in CSS to create inner spacing inside an element.

![padding](https://github.com/user-attachments/assets/551c29fa-8f98-445d-9d8d-f20ef97b53a6)

### HTML Horizontal Rules:
- The hr tag defines a thematic break in an HTML page, and is most often displayed as a horizontal rule.
- The hr element is used to separate content (or define a change) in an HTMl page:

![hr tag](https://github.com/user-attachments/assets/5cdab91a-d111-4d69-8254-076611150e1f)

### HTML Line Breaks:
- The HTML br element defines a line break.
- Use br if you want a line break (a new line) without starting a new paragraph:

![br tag](https://github.com/user-attachments/assets/bcdf1a7e-1068-4ff7-8a73-0ae5831dcc58)
- The br tag is an empty tag, which means that it has no end tag.

### HTML IFrames:
An HTMl iframe is used to embed another webpage inside the current webpage. It allows you to display videos, maps, or external websites within a section of your page.

![iframes](https://github.com/user-attachments/assets/de951163-2ffb-43df-a7dd-7f8bfd08b29a)




