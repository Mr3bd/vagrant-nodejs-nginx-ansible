# 🚀 Vagrant Node.js App with NGINX & Ansible

A simple development environment powered by **Vagrant**, provisioned with **Ansible**, running a basic **Node.js** app behind **NGINX** as a reverse proxy.

## 📦 Stack
- Ubuntu 22.04 (via bento/ubuntu-22.04)
- Node.js 18
- PM2 for Node.js process management
- NGINX as reverse proxy
- Ansible for provisioning

## 🔧 Features
- Automatic installation of Node.js & NGINX
- Reverse proxy with NGINX to Node.js
- Simple Hello API response
- Uses PM2 to manage the Node.js process

## 🖥️ How to Run

```bash
git clone https://github.com/mr3bd/vagrant-nodejs-nginx-ansible.git
cd vagrant-nodejs-nginx-ansible
vagrant up
```

Then open:
[http://localhost:8080](http://localhost:8080)

You should see:
Hello from Vagrant + Ansible + Node.js!

## 🤝 You Can:
- Fork this repo
- Modify the app to fit your needs
- Use it for learning or development

----

## 👨‍💻 Author

[Abdullrahman Wasfi](https://github.com/Mr3bd)

Made with ❤️ using Vagrant, Ansible, and Node.js