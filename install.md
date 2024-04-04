<samp>

  
# Installation
This guide provides instructions for setting up the operating system environment, including installation and configuration steps. Follow these steps to prepare your system for running the operating system using the Bochs emulator.

## Prerequisites
Before you begin, ensure that you have the following prerequisites installed on your system:

- [Bochs](https://bochs.sourceforge.io/) emulator
- Operating system codebase (already provided)

## Installation Steps

1. **Download Bochs:**
   - Visit the [Bochs website](https://bochs.sourceforge.io/) and download the latest version of Bochs for your operating system.

2. **Install Bochs:**
   - Follow the installation instructions provided with the Bochs package to install it on your system.

3. **Extract Operating System Codebase:**
   - Extract the provided operating system codebase from the zip file.

## Configuring Bochs

Once you have installed Bochs and extracted the operating system codebase, follow these steps to configure Bochs:

1. **Configuration File:**
   - Locate the Bochs configuration file (usually named `bochsrc.txt`).
   - Open the configuration file in a text editor.

2. **Set Disk Image:**
   - Add the path to the disk image file of the operating system to the configuration file. Place the boot img in the same directory as the OS files.
     ```
     ata0-master: type=disk, path="path/to/disk/image"
     ```

3. **Set Boot Options:**
   - Set the boot options to boot from the disk image.

     ```
     boot: disk
     ```

4. **Set Other Options (Optional):**
   - Configure other options such as memory size, display options, etc., based on your requirements.

5. **Save Configuration:**
   - Save the changes to the configuration file.

## Compiling the Operating System
Once you configured bochs, Compile the OS by executing (linux)
```
./build.sh
```
and on mac:
```
./build(mac).sh
```

## Running the Operating System

Once Bochs is configured, you can start the emulator and run the operating system by executing the following command:

```
bochs -q
```

This command will launch Bochs with the configured settings, and the operating system should start running within the emulator.

## Conclusion

You have successfully set up the operating system environment and configured Bochs for running the operating system. You can now start exploring and working with the operating system.
For any issues or questions, refer to the [Bochs documentation](https://bochs.sourceforge.io/documentation.html) or consult the provided codebase.



</samp>
