# IP Address Grouping Tool

This simple Python script takes a subnet mask as input and reads a list of IP addresses from a text file. It then calculates the network address for each IP based on the provided subnet mask and groups the IP addresses accordingly.

## Usage

1. **Input Subnet Mask**: Run the script and provide a subnet mask when prompted. The subnet mask should be in the range of 0-32.

    ```bash
    Enter the subnet mask (0-32): [your_subnet_mask]
    ```

2. **Input File Path**: The script reads IP addresses from a text file. Ensure that your file has a valid list of IP addresses, each on a new line. The default file path is set to `C:\your\path\to\ip_addresses.txt`. You can modify the `file_path` variable in the script if your file is located elsewhere.

3. **View Results**: The script will output the IP addresses grouped by their calculated network addresses. Each group corresponds to a subnet based on the provided subnet mask.

## How It Works

The script uses bitwise operations to calculate the network address for each IP address. It then groups the IP addresses based on their respective network addresses.

## Example

For example, if your `ip_addresses.txt` file contains the following IP addresses:

192.168.1.1
192.168.1.2
192.168.2.1

And you input a subnet mask of `24`, the script might output:

Subnet 192.168.1.0/24:
192.168.1.1
192.168.1.2

Subnet 192.168.2.0/24:
192.168.2.1


## Important Note

Ensure that the input file contains valid IP addresses and that the subnet mask provided aligns with your network configuration.

Feel free to customize the script or integrate it into your projects as needed.

Happy networking!
