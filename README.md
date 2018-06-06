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

Currently node can't understand version ES6 commands
run the following command to solve the problem

- `npm install enhanced-resolve@3.3.0`

