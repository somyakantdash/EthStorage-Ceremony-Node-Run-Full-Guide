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
## If u Runa Node in VPS One-Click Deployment in VPS 
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

## 🔶For Next Day Run This Command

#1 Open WSL then Put this Command 
```
cd ~/trusted-setup-tmp
```
```
phase2cli contribute -c ethstorage-v1-trusted-setup-ceremony
```
* Press **Enter** for random input

---

### If Your Showing These anyone of these Error then Put Below Command

![6127616883743114503 (1)](https://github.com/user-attachments/assets/2b90dabe-4678-46f2-81a0-93b37462e9f2)

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
