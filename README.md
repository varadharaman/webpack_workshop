# webpack workshop on windows
webpack_workshop

## Webpack Workshop Setup Instructions
Following are the steps for installation of Webpack related software on Windows systems.
Please read the complete instructions and follow exactly as per the instruction and install exactly in the mentioned folders.  
Note:    Drive:  mentioned below is C: or D: or E: or F: etc. wherever space is available for installation. 

1)	Install Node.js [ node-v4.4.2-x86.msi  - Windows 32 bit installer ].
a.	https://nodejs.org/dist/v4.4.2/node-v4.4.2-x86.msi 

2)	Install Notepad++ 6.9.1 [ npp.6.9.1.Installer.exe ].
a.	https://notepad-plus-plus.org/repository/6.x/6.9.1/npp.6.9.1.Installer.exe 

3)	Install the latest version of Google Chrome.
4)	You can create a folder webpack_workshop under Drive:\

5)	If not present, create  the folder “npm” under C:\Users\<username>\AppData\Roaming.    If the folder “AppData” is not shown, Go to File Explorer | Organize | Folder and search options | View tab. Click on the radio button “Show hidden files, folders, and drives”.

6)	Goto “Node.js command prompt”. (Use  the shortcut present under the “Node.js” traversed through “Start | All Programs”.
a.	Change directory to Drive:\webpack_workshop

7)	IMPORTANT NOTE: This step is required only if you are installing behind Wipro proxy. Otherwise, do not issue the below commands.
If behind Wipro proxy, Configuring proxy for node.js is important using npm config. Only if proxy is configured, “npm  install” will work properly.
```
npm config set proxy http://LDAP-ADUserID:LDAP-ADpassword@proxyname:port
npm config set https-proxy http://LDAP-ADUserID:LDAP-ADpassword@proxyname:port
```

IMPORTANT (OPTIONAL STEP – NOT A REGULAR ONE) :  In case, you have already set the proxy config wrongly and want to run the remaining commands from Direct Connection To Internet, then to delete the proxy configuration, execute the following commands.
```
npm config delete proxy
npm config delete https-proxy
```

8)	Ensure you are in the directory Drive:\webpack_workshop in Node.js command prompt.
Run the following commands
```
npm init -y
npm install --save-dev autoprefixer-loader@3.2.0
npm install --save-dev babel-loader@6.2.2
npm install --save-dev babel-preset-es2015@6.5.0
npm install --save-dev babel-preset-react@6.5.0
npm install --save-dev css-loader@0.23.1
npm install --save-dev extract-text-webpack-plugin@1.0.1
npm install --save-dev jshint-loader@0.8.3
npm install --save-dev less-loader@2.2.2
npm install --save-dev sass-loader@3.1.2
npm install --save-dev strip-loader@0.1.2
npm install --save-dev style-loader@0.13.0
npm install --save-dev url-loader@0.5.7

npm install -g webpack@1.12.14
npm install -g webpack-dev-server@1.14.1
npm install -g http-server@0.9.0
```

9)	Be in Node.js command prompt and ensure you are in  the directory Drive:\webpack_workshop  and then Create a directory “code” under <Drive>:\webpack_workshop

10)	During the training session on Webpack, while trying out each concept, you can create a separate sub-folder under “code” to try out each concept.
