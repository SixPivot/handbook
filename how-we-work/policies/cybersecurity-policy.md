# Cybersecurity Policy

## Purpose

The purpose of this cybersecurity policy is to protect our customer’s data as well as the data we use to do business within SixPivot. We all play a part in protecting the sensitive information we deal with. This policy contains guidelines for securely managing credentials, customer data, and your laptop.

This policy applies to everyone at SixPivot, as we all interact with systems that process and store sensitive information.

This policy does not contain development guidelines. For that we have the dev wiki, our professional development days, and the combined experience of the team.

## Guidelines

### Laptops and Desktops

These guidelines apply to any computer you use for work, such as a laptop or desktop. Follow the client guidelines and policies for client issued laptops.

1. Turn on device encryption. On Windows use [BitLocker](https://support.microsoft.com/en-us/windows/turn-on-device-encryption-0c453637-bc88-5f74-5105-741561aae838), on Mac use the [Disk Utility](https://support.apple.com/en-au/guide/disk-utility/dskutl35612/mac), and on Linux use [cryptsetup](https://gitlab.com/cryptsetup/cryptsetup) with Linux Unified Key Setup (LUKS).
2. Install security software that actively monitors your device for threats.
3. Set a lock screen with a password, PIN, or biometrics. Do not share your password/PIN with anyone, or let anyone use your login.
4. Recommend disabling content in notifications (e.g., show Slack notifications without the message content). This will ensure that no confidential or private information is accidentally shared during a screen sharing session.
5. When you no longer use your laptop for work, e.g., passing it on to a family member, selling, using as a paper weight, you need to perform a full disk format (the option where data is completely erased, not marked as deleted.

<details>

<summary>Procedure: Enabling device encryption on Windows</summary>

📝 You need Windows 10 or 11 Pro edition to enable BitLocker.

You can enable BitLocker yourself following [the Microsoft instructions](https://support.microsoft.com/en-us/windows/turn-on-device-encryption-0c453637-bc88-5f74-5105-741561aae838), or follow these steps. Just remember to store your BitLocker recovery key in your SixPivot OneDrive personal files.

#### Step-by-step instructions

1.  Search “BitLocker” or select Start > Control Panel > System and Security > BitLocker Drive Encryption\


    <figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>
2. Choose ‘Turn on BitLocker’
3.  If you get an error that says “This device can’t use a Trusted Platform Module” then read the steps below “BitLocker Without Trusted Platform Module”\


    <figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>
4. Click Next through each step, accepting the default settings. Windows will suggest you back up your data before proceeding.
5. When it asks you to back up your recovery key, choose ‘Print the recovery key,’ and in the print dialog choose “Microsoft Print to PDF” and click Print. Enter “BitLockerRecoveryKeys.pdf” as the file name.
6.  **You must upload the recovery keys to your personal SixPivot OneDrive files.**

    📝 Every now and then Windows might ask you to enter your recovery key if it detects a change to the system (BIOS changes, partitioning the drive). By storing your keys in OneDrive, you can access them from your mobile.
7. Click next on the remaining steps. The last screen will have an option ‘Run BitLocker system check.’ Check this, then click Continue. BitLocker will show a pop up asking you to restart, once you restart BitLocker will be enabled.
8.  The BitLocker settings page should tell you if encryption is enabled.\


    <figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

#### BitLocker Without Trusted Platform Module

A Trusted Platform Module (TPM) is a piece of hardware that comes with modern laptops. It simplifies the BitLocker set up but is not mandatory. These steps will turn on BitLocker without a TPM.

1.  Search “Local Group Policy Editor” and open “Edit group policy”:\


    <figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>
2.  Open Computer Configuration > Administrative Templates > Windows Components > BitLocker Drive Encryption > Operating System Drives then open the setting ‘Require additional authentication at startup’.\


    <figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>
3.  Select ‘Enabled’ then select OK to close the settings\


    <figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>
4.  Now follow the steps to enable BitLocker. You will see an extra step in the process that will ask you to choose how to unlock your drive at startup. Choose ‘Enter Password’\


    <figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>
5.  Windows will ask you for this password every time you start your device:\


    <figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>
6. This password decrypts your drive each time you start your computer. You will still be asked to log in to Windows like usual after this.

</details>

<details>

<summary>Procedure: Removing data from Windows</summary>

When you dispose of your laptop, such as selling it or giving it to a friend or family member, make sure to delete your user profile.

The procedure is listed in the steps below, but the approach is as follows:

* Create a new local administrator account
* Log in with that new account and delete your profile
* Delete work related data that is not stored in your user profile directory

#### Step-by-step instructions

1. Search “Add user” > “Add, edit, or remove other users” > Add someone else to this PC or Control Panel > User Accounts > User Accounts > Manage Another Account > Add a new user in PC settings > Add someone else to this PC
2.  Choose “I don’t have this person’s sign-in information”\


    <figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>
3. Choose “Add a user without a Microsoft account”
4. Enter a new username, if you are passing on this laptop enter the new owner's name, or if you are just deleting your old profile enter something like “New Administrator"
5. Enter a password and fill out the security questions. Then create the new user.
6.  Click the new user you just create and select Change account type\


    <figure><img src="../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>
7.  Choose Administrator\


    <figure><img src="../../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>
8.  Log In to the new account. Go Start > Click your username > Sign out\


    <figure><img src="../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>
9.  Log in to the new account (bottom left will display your old profile and the new one you just created)\


    <figure><img src="../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>
10. Repeat step 1 to open the user management screen.
11. Select your old profile and click Remove.\


    <figure><img src="../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>
12. As the warning says, this will delete all the data associated with that account. If you have any personal data you want to back up do this first, then click “Delete account and data”\


    <figure><img src="../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>
13. Make sure you manually delete any work-related data that you were storing outside of your user profile, such as directories under C:\ drive, or another hard drive.

</details>

<details>

<summary>Procedure: Enabling disk encryption on Mac</summary>

Follow the steps outlined [here](https://geekgirltech.com/how-to-enable-disk-encryption-on-mac-and-windows-o-s/).

</details>

<details>

<summary>Procedure: Enabling disk encryption on Linux</summary>

An overview of the procedure:

* For existing installations, back up your home (\~) directory somewhere (USB / another partition)
* Create a small (1.8G) ext4 partition that will be mounted at /boot when we install Linux
* Create a new ext4 partition that will store your encrypted swap and root partitions
  * Encrypt this ext4 partition with LUKS
  * Within this partition create a logical volume group with two volumes:
    * A swap volume
    * A root volume (to store OS and data)
* Install Linux on the root volume, specify the swap volume as swap and mount the 1.8G partition at /boot
* Configure your new installation to prompt for the encryption passphrase
* For existing installations overwrite your home directory from the backup.

The above procedure has been confirmed on Ubuntu (22.04) only, and basically followed the steps in [this guide](https://www.mikekasberg.com/blog/2020/04/08/dual-boot-ubuntu-and-windows-with-encryption.html) (skipping straight to Phase 3 about partitioning the drive).

It is possible to encrypt an existing disk without reinstalling, but this has not been proven and may lose to a broken install; [here be dragons](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/8/html/security_hardening/encrypting-block-devices-using-luks_security-hardening#encrypting-existing-data-on-a-block-device-using-luks2_encrypting-block-devices-using-luks).

Here is a screen shot of the partition table that contains a Windows 11 installation alongside an Ubuntu installation. Both OSs have disk encryption turned on.

![](<../../.gitbook/assets/image (28).png>)

</details>

### 2. Passwords

1. Store client account as well as SixPivot account credentials in the SixPivot credential manager linked to your private vault.
2. Enable MFA on client email and client accounts.
3. Change default passwords. If the client IT can only set your password, share a one-time-link to the password in your credential manager for them to set as your password.
4. Store client collateral in the SixPivot client folder on SharePoint.
5. Store shared credentials in the SixPivot credential manager linked to the client vault. Shared credentials are those required by the project team to onboard and access the application(s) they are working on (database credentials, application log ins, etc.).
6. Discourage the use of generic accounts. If clients provide us with a “sixpivot” shared account, we should strongly encourage them to create individual accounts for each of our team members. The use of generic accounts is bad practice as it limits the ability to audit user actions reliably.
7. Clients will often provide us with global admin (Azure) or root account (AWS) access to their cloud platforms. We should only use these credentials to set up delegated access to cloud platforms. For example, we will create specific “named” Azure AD or IAM users for each of our team who needs to access the platform.
8. Regular user access reviews will be undertaken every three months to ensure that SixPivot team members who no longer require access to customer data have been removed. This is mostly applicable to customers where we have a long-term support agreement (see 3.2).

<details>

<summary>Procedure: 1Password Private vs Client vaults</summary>

In 1Password you will see your private vault and many different vaults, one for each client.

*   Store your account credentials in your “Private” vault. Account credentials are the log ins that require your SixPivot email or client email to log in to email, Teams, Miro etc. Your private vault is accessible only to you.\


    <figure><img src="../../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>
* Shared client secrets are stored in the client vault. These can be accessed by anyone at SixPivot. A shared client secret is anything except your account credentials. Examples are log ins for the application you are building, database credentials for each environment, Seq logins, build server tokens, etc.

</details>

<details>

<summary>Procedure: Securely sharing credentials</summary>

When you need to share credentials from 1Password, do not copy the credentials and paste them into email or chat, use the [1Password secure share](https://support.1password.com/share-items/) feature.

#### Recommended settings:

**Only some people**

Enter their email address(es). You then share the link with the audience, and they will need to enter their email address. If their email matches, they will receive a verification code via email.

![](<../../.gitbook/assets/image (25).png>)

![](<../../.gitbook/assets/image (26).png>)

**Can be viewed only 1 time**

Mission Impossible self-destruct feature invalidates the link once it has been viewed.

![](<../../.gitbook/assets/image (27).png>)

&#x20;

</details>

### 3. Data

1. Delete source code from your device and delete credentials from your personal account when the engagement ends.\
   The end of the engagement should be after you have completed the handover, onboarding and training and you are no longer expected to provide support to the customer (see 3.2).
2. When we have an agreement (formal or informal) with the client to provide support, do not delete the credentials or source code. This ensures we can respond quickly to urgent support requests. When the agreement ends then delete the source code and credentials (see 3.1).
3. It’s encouraged to keep code snippets for your personal knowledge base or to share with the team. Do not keep the entire source code, unless that is something we agreed to with the customer, such as to save time on boarding in the future, or when we host the customer's source code in the SixPivot repository. What we normally want to keep is useful patterns we applied for that job, not the whole code base itself.
4. To avoid accidental sharing of customer-identifying text from the code snippets, remove these when collecting code snippets.

### 4. Incidents

1. Notify the principal leadership team (PLT) about suspected or confirmed breach of customer data on your device. This includes accidental loss or theft of laptop.
2. Change your account credentials in case of a breach. This includes your SixPivot account, as well as the client accounts.
3. Security incidents that occur within the customer environment, such as DOS, threat intrusion or any other cyber incident can be reported directly to the relevant client contact(s). Keep the SixPivot project team in the loop as a second priority to managing the incident with the client.
