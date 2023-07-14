# Shraddha_assignment
create a Amazon account 
Note: We recommend saving the private key file as a .pem format with RSA encryption.

Create a security group. Note, we recommend adding a rule for HTTP, HTTPS, RDP, and All ICMP - IPv4.

Launch the instance
To create a new virtual machine instance on AWS, follow these steps:

Open the Amazon EC2 console.

From the EC2 console dashboard, select Launch Instance.

Provide a name for the VM instance. For this tutorial, we’ll use the name “RhinoComputeVM”.

Under the section titled Application and OS Images, click on the button to Browse more AMIs. The Choose an Amazon Machine Image (AMI) page displays a list of basic machine configurations (AMIs) to choose from. In the filter on the left, select All Windows to show only Windows AMIs. Select the AMI for Windows Server 2019 Base or later. Note that these AMIs are marked Free tier eligible. We will be using Windows Server 2019 Base for this tutorial, but Windows Server 2022 Base has been tested and is supported./images/AWS_Setup_01.png
In the Instance Type section, select the t2.micro instance type (default) or a larger instance type if needed. Note: the t2.micro instance type is elegible for the free tier. In regions where t2.micro is unavailable, you can use a t3.micro* instance under the free tier./images/AWS_Setup_02A.png
In the Key Pair (login) section, select the key pair name that you created in step 2 of the prerequisite section prerequisite section from the drop-down list.

In the Network Settings section, under the Firewall (security groups) choose the Select existing security group radio button. Then, under the Common Security Groups drop-down list, select the security group you created in step 3 of the prerequisite section. If the Auto-assign public IP setting is not set to Enable, click on the Edit button on the top-right of this section panel and change this setting appropriately./images/AWS_Setup_10.png
In the Configure storage section, select the default amount of storage for this instance.

Now, on the far right select the Launch Instance.

A confirmation page lets you know that your instance has successfully launched. In the top-most menu which reads EC2 > Instances > Launch an instance, select the Instances menu item to view the instances console window./images/AWS_Setup_09.png
On the Instances screen, you can view the status of the launched instance. The instance should automatically be running after launch, but if not select the instance row checkbox and then select the Instance State menu item at the top. Select Start Instance to start the virtual machine.

With the instance row selected, click the Connect button in the top menu.

On the Connect to instance page, select the RDP client tab. Select the Download remote desktop file and save the .rdp file somewhere on your local computer.

Next, select the Get password button.

Choose Upload private key file and navigate to the private key (.pem) file that you created when you launched the instance.

Choose Decrypt Password. The console displays the default administrator
