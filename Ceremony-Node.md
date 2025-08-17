# EthStorage Ceremony Node Run Full Guide (PC and VPS)

### Offical Docs Guide - https://blog.ethstorage.io/join-the-ethstorage-v1-trusted-setup-ceremony/

----

## 🧰 Prerequisites
### Before getting started, make sure you have the following:
	
 * GitHub account (for authentication)
 * Account age ≥ 1 month  
 * At least 1 public repository  
 * Follow ≥ 5 accounts & have ≥ 1 follower

-------------
## If u Run a Node in VPS
* Xorek Cloud [HERE](https://tinyurl.com/5b6cn7zs)
   - Buy ur VPS according to Node System Requremnts > Then Follow Below Code Step by Step
* Buy VPS & Run Node:- https://www.youtube.com/channel/UCgyz28ZN5EKLVXGI4XaPZKA
   - HOw to Buy VPS or How to Run any Node in VPS then Watch Above Video
------------

---

1️⃣ Dependencies for WINDOWS & LINUX & VPS
```
sudo apt update && sudo apt upgrade -y
sudo apt install -y curl git build-essential
```

2️⃣ Install Node JS & NPM
```
curl -fsSL https://deb.nodesource.com/setup_18.x | bash -
apt install -y nodejs
npm install -g npm@9.2
```
```
node -v
npm -v
```

3️⃣ Make Directory
```
mkdir ~/trusted-setup-tmp && cd ~/trusted-setup-tmp
```

4️⃣ Install Phase2 CLI
```
npm install -g @p0tion/phase2cli
```

5️⃣ Verify CLI Installation
```
phase2cli --version
```

6️⃣ Authenticate with GitHub
```
phase2cli auth
```

* Follow the browser link shown in the terminal
* Login to GitHub & authorize p0tion to access Gists
* Return to terminal

**OR**

* Visit **[https://github.com/login/device](https://github.com/login/device)**
* Enter the code from ur terminal
* Click **Authorize ethstorage**
* Allow **Read & Write access to GitHub Gists** in permissions

For VPS Only
```
apt install screen -y
```
```
screen -S ceremony
```
- PRESS CTRL+A+D (to run ur node continuously)
- To check ur Node Again
```
screen -r ceremony
```

7️⃣ Start Node
```
phase2cli contribute -c ethstorage-v1-trusted-setup-ceremony
```

* Press **Enter** for random input

8️⃣ Final Step

- Once all commands are run, wait for your queue.  
- When your turn comes, the tool will process your contribution.  
- Done! 🎉 You have successfully contributed to the EthStorage V1 Trusted Setup Ceremony.

---

## 🔶For Next Day Run This Command (Only for Local PC)

#1 Open WSL then Put this Command 
```
cd ~/trusted-setup-tmp
```
```
phase2cli contribute -c ethstorage-v1-trusted-setup-ceremony
```
* Press **Enter** for random input

---

---

### If u r seeing this error or Stuck ur Node

![6127616883743114531 (1)](https://github.com/user-attachments/assets/4d113367-c8bf-4e65-91be-27a5a7975d7b)
![Picsart_25-08-17_14-57-28-991](https://github.com/user-attachments/assets/27e4ceae-7b1d-4e96-be3d-7ab00ce8a589)

* Discord: https://discord.gg/BKnJY8WZ2t

```
GITHUB EMAIL: email
GITHUB USERNAME: username
```

  - Join Discord > Verify Urself 
  - Go to #technical-discussion channel > Put ur Stuck or Queue Sscreenshot, GitHUb email and username in this format, also tag @molaokp on your message, so you can get Verified.


### If u r seeing this error then Put Below Command

![6127616883743114503 (1)](https://github.com/user-attachments/assets/7cb501c7-a892-40b9-ae45-282f51b1c662)

```
npm uninstall -g @p0tion/phase2cli
npm install -g @p0tion/phase2cli
phase2cli auth
```
after that write that START NODE command

---

## Stop & Delete node
```
phase2cli clean
phase2cli logout
cd ~ && rm -rf ~/trusted-setup-tmp
```
