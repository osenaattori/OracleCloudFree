
# How to get free cloud VPS from Oracle 
--- How to claim a 24gb 4ocpu arm server for free ---

1. Navigate to https://signup.cloud.oracle.com/ and Create an account, the country/territory options you choose are important, since you can only create a free server in your selected home region.

2. Navigate to https://cloud.oracle.com/compute/instances and click "Create Instance"

3. Customize the instance like so:

	Name: your preference
	Compartment: leave default
	Placement: Any (choose the one you can)
	Image and shape:
		Image: Canonical Ubuntu (not minimal)
		Shape:
			Instance type: Virtual Machine
			Shape series: Ampere
			OCPU: 4
			Memory: 24GB

	Networking:
		Primary network: Create new virtual cloud network
		Subnet: Create new public subnet
		Public IP Address: Assign a public IPv4 address

	Add SSH keys: Add / generate your SSH keys, don't choose "No SSH keys" please

	Boot volume:
		Specify a custom boot volume size: True
		Boot volume size (GB): 200 (or 199 to be safe)

4. Click "Create"
5. Start your server and connect to it
6. Setup your firewall, create your own account and remove the default one, etc security stuff.

