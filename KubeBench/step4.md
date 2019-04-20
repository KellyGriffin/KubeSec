Let’s now run Kube-Hunter

We will now download and install the AquaSec OpenSource project called Kube-Hunter  This will run on the Cluster and allow us to run a scan that shows any vulnerabilities. 

Run the following to identify the IP Address - you will need this for the Scanning.

`hostname -I | awk '{print $1}'`{{execute}}

Got to https://kube-hunter.aquasec.com/ and enter your Email Address - this will create a Docker command for you to copy and paste into your Minikube environement.

Press Enter and type 1 for Remote Scanning

Enter the IP Address you copied before

Once complete - head back to the Kube-Hunter page and click on the Hyperlink - `After you run this command, results will appear here.`

Review and Enjoy