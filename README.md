# Not Working Anymore


# Steam Bulk Trade Bot
This is a simple Steam trade bot script written in Node.js using the steam-user, steamcommunity, steam-totp, and steam-tradeoffer-manager modules. It logs in to multiple Steam accounts provided in a text file and sends a trade offer containing all the items in the account's inventory to a predefined trade link.

# Installation
1. Clone the repository using git clone https://github.com/Stiphr/Steam-Bulk-Trade-Bot or download the zip file and extract it to a directory of your choice.
2. Install the required modules by running **npm install** in the directory where the repository was cloned or extracted.
3. Edit the **accounts.txt** file in the root directory and replace the sample account information with your own Steam account details in the format **username:password:2fa_token:identity_secret** (identity_secret can be left blank if not using mobile authentication).
4. Add your account's tradelink in **tradelink.json** file in the root directory

# Usage
Once the script is running, it will log in to each account one by one, wait for 12 seconds, and then log off. It will repeat this process for all accounts in the **accounts.txt** file. When a successful login occurs, the bot will get the inventory of the account and send a trade offer containing all the items to the predefined trade link in the **tradelink.json** file. If the trade offer requires confirmation, the bot will automatically accept it using the identity secret provided in the **accounts.txt** file.

# Disclaimer
This script is provided for educational purposes only. Using multiple accounts to gain an unfair advantage in trading is against the Steam Subscriber Agreement and can result in a ban or other penalties. Use at your own risk
