# GPUCloud
* [Sign up and login the Genesis Cloud](#sign-up-and-login-the-genesis-cloud)
* [Create an instance for computation](#create-an-instance-for-computation)
  * [Step 1: Add your credit card](#step-1-add-your-credit-card)
  * [Step 2: Create and register a `ssh` key](#step-2-create-and-register-a-ssh-key)
  * [Step 3: Create and configure a GPU instance](#step-3-create-and-configure-a-GPU-instance)
* [Use the created instance](#use-the-created-instance)
* [Install Required Packages](#install-required-packages)


## Sign up and login the Genesis Cloud

[Sign-up](https://account.genesiscloud.com/signup/HX6DfDGFuxSn0sSmPmSKB) Genesis Cloud using your email address and [login](https://account.genesiscloud.com/signin/tGu7mwKi5_f3naXxcomYy) Genesis Cloud Account using your credentials. 

   After login, you can access the dashboard.
   ![2020-11-04 (5)](https://user-images.githubusercontent.com/29531232/98150935-6bd6eb80-1ef5-11eb-9dff-cfe7e71e7bec.png)

## Create an instance for computation 
To compute your code using any instance do the following steps

 * ### Step 1: Add your credit card
   Before creating an instance, we need to add the details of credit card. 
   ![billing](https://user-images.githubusercontent.com/29531232/98151665-8f4e6600-1ef6-11eb-9444-f9bb554f31a5.png)
 
 * ### Step 2: Create and register a `ssh` key
   In this step, first create `ssh` key. To generate `ssh` key in Ubuntu do the following steps
   ```sh
   pratik@PRATIK-YOGA:~$ ssh-keygen
   Generating public/private rsa key pair.
   Enter file in which to save the key (/home/username/.ssh/id_rsa):
   Created directory '/home/username/.ssh'.
   Enter passphrase (empty for no passphrase):
   Enter same passphrase again:
   ```
   This is the last step in the creation process. You now have a public and private key that you can use to authenticate.
   ```
   Your identification has been saved in /home/username/.ssh/id_rsa.
   Your public key has been saved in /home/username/.ssh/id_rsa.pub.
   ```
   Now, we need to register the generated `public ssh key`(.pub) in genesis cloud. To do this, go to the **Account section** in the navigation menu, select **Keys and Tokens**. In the **SSH keys** section, click `Add new Key`.
   ![sshkey](https://user-images.githubusercontent.com/29531232/98155932-10106080-1efd-11eb-8965-a549a70491fe.png)
   
   A popup window will appear
   ![popup](https://user-images.githubusercontent.com/29531232/98157375-4818a300-1eff-11eb-9892-96bb6b984d77.png)
   In that window, upload the generated public key(`.pub`) file. 
   
  * ### Step 3: Create and configure a GPU instance
    To do this, go to the **Compute section** in the navigation menu, click **Instances**. Then, click **Create New Instance**.
    ![2020-11-05 (1)](https://user-images.githubusercontent.com/29531232/98163640-16a4d500-1f09-11eb-8dfc-8a0b7b465190.png)
    
    
    Now, you can change the host name if required and click on **Preconfigured** image. 
    ![2020-11-05 (2)](https://user-images.githubusercontent.com/29531232/98164219-f9bcd180-1f09-11eb-9edc-a4405c9c718b.png)
    
    
    Now, generate the passowrd and save it for further use
    ![2020-11-05 (5)](https://user-images.githubusercontent.com/29531232/98164573-810a4500-1f0a-11eb-97f1-c66e659b733f.png)
    
    
## Use the created instance 
   Now, the instance is created. Click on the instance and the get the details of `ssh` command to use that instance.   
   ![2020-11-05 (8)](https://user-images.githubusercontent.com/29531232/98167328-e6f8cb80-1f0e-11eb-8ea8-56c9354c0b9c.png)
    
   ![2020-11-05 (7)](https://user-images.githubusercontent.com/29531232/98167432-11e31f80-1f0f-11eb-93fa-d9c1618e4480.png)

    


  ## NOTE: `pip` and `conda` both are used to install packages in your local system. But to install package in any specific environment use `conda`.  
