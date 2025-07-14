## 25/06/2025
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

## 26/06/2025

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

   ## 27/06/2025
