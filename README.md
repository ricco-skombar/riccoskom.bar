# riccoskom.bar 

Manually intallation on a CentOs 7 Server:

----------------

Install Git:

- `yum -y install git`
- `git --version`

Install Nano

- `yum -y install nano`
- `nano --version`

Install node.js with epel

- `yum -y install epel-release`
- `yum -y install nodejs`
- `node --version`

Install npm

- `yum -y install npm`
- `npm --version`

Clone the project

- `git clone https://github.com/riccoDeveloper/riccoskom.bar.git`

Install npm-dependencies in the project-directory

- `cd riccoskom.bar/`
- `npm install`

Currently node can't understand version ES6 commands.
Run the following command to solve the problem

- `npm install enhanced-resolve@3.3.0`

Now the server should start without problems.
Test it with the following command:

- `npm run start`

Install pm2 with typscript support

- `npm install pm2 -g`
- `pm2 install typescript`

Now start the server with pm2 command

- `pm2 start src/server.ts`

Generate a startup script with pm2 so the server will restart
after a reboot of the system or crash of the app

- `pm2 startup centos`
- `pm2 save`

Reboot the system and check if pm2 starts the server automatically

- `reboot`
- `cd riccoskom.bar/`
- `pm2 status src/server.ts`


