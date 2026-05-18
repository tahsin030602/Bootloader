Extract the contents of the `duos24` folder in the same directory where the `Bootloader03_30_60.patch` file is located.

Then run the command
```bash
patch -p0 < Bootloader03_30_60.patch
```

#### Run the Python server:
- Write the current update version inside the file `version.txt`
- Specify the path to the current OS version binary inside the file `file_path.txt`
- Run the Python Server using command:
```bash
python main_server.py
```

#### Load the Bootloader Program into the device following these steps:
- Navigate to the `duos24/src/compile` directory.  
- Open that location in the command line.  
- Use the command `make all` to create the binary file.  
- Use the command `make load` to load the binary file onto the STM32F446RE MCU.  
