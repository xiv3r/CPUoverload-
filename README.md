# <h1 align="center"> CPU OVERLOADING
<br><br>



- ### Direct execution from Raw

      wget -qO- https://raw.githubusercontent.com/xiv3r/CPUoverload/main/CPUoverload.sh | sudo sh


- ### Manual Installation

      git clone https://github.com/xiv3r/CPUoverload.git

      cd CPUoverload

      chmod +x CPUoverload.sh
   
      sudo sh CPUoverload.sh


- ### Automate through Crontab

      cd CPUoverload
  
      sudo cp CPUoverload.sh /etc/

      chmod +x /etc/CPUoverload.sh

      sudo crontab -e

  Add:
  
      # Execute every 1 minute
      * * * * * /etc/CPUoverload.sh

      # Execute After rebooting the system
      @reboot /etc/CPUoverload.sh

  # Load after Boot
     * persistent

      wget -qO- https://raw.githubusercontent.com/xiv3r/CPUoverload/main/CPUoverload.sh | sudo sh
