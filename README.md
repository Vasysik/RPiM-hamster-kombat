# RPiM-hamster-kombat Module for RPiModules

## Description

RPiM-hamster-kombat is a module for RPiModules that allows you to set up and run a mining operation for hamsters on your Raspberry Pi (RPi). This module is designed to enhance the functionality of your [RPiModules](https://github.com/Vasysik/RPiModules).

## Installation

1. Clone the RPiM-hamster-kombat module from the GitHub repository to the 'modules' directory within your [RPiModules](https://github.com/Vasysik/RPiModules).

   ```
   git clone https://github.com/Vasysik/RPiM-hamster-kombat.git /path/to/RPiModules/modules/hamster
   ```

2. Open the `modules.json` file located in your RPiModules directory and add the following configuration for the hamster module:

   ```json
   "hamster": {
       "route": "hamster",
       "icon": "hamster/static/hamster_icon.png",
       "name": "hamster",
       "enable": true
   }
   ```

3. Configure the `hamster_config.json` and `hamsterkombat/config.json` files within the hamster module according to your requirements.

4. Configure and Install the `hamster.service` service for your [RPiModules](https://github.com/Vasysik/RPiModules).

   ```
   sudo cp /path/to/RPiModules/modules/hamster/hamster.service /etc/systemd/system/
   sudo systemctl daemon-reload
   sudo systemctl enable hamster.service
   sudo systemctl start hamster.service
   ```

## Usage

Once the installation and configuration are complete, you can access the hamster module through your [RPiModules](https://github.com/Vasysik/RPiModules) web interface. Use the provided configuration files to customize the hamster mining operation according to your needs.

## Contributing

Contributions to the RPiM-hamster-kombat module are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue on the GitHub repository. Pull requests are also encouraged.
