# SwitchHosts!
Based on issue `#480 建议增加云账号或云同步公共`,now supports pulling multiple configurations remotely.

## How can do this

- first  
Prepare configuration files in the cloud
- second  
You need to select cloud from the add new rule interface,as follows:  
<img src="https://raw.githubusercontent.com/Medivh-C/SwitchHosts/master/screenshots/add_new_cloud_rule.png" alt="Capture" width="480">  

## How to write cloud configuration files
You can write it like this:
```json
[
  {
    "title": "test1",
    "description": "This is test host1",
    "rules": [
      {
        "ip": "127.0.0.1",
        "host": "www.baidu.com"
      },
      {
        "ip": "127.0.0.2",
        "host": "www.sina.com.cn"
      }
    ]
  },
  {
    "title": "test2",
    "description": "This is test host2",
    "rules": [
      {
        "ip": "127.0.0.1",
        "host": "www.google.cn"
      }
    ]
  }
]
```
You will synchronize 2 configurations from the cloud, named Test 1 and Test 2.

### The screenshot corresponding to the above configuration file is as follows
<img src="https://raw.githubusercontent.com/Medivh-C/SwitchHosts/master/screenshots/cloud_test.png" alt="Capture" width="960">   

<img src="https://raw.githubusercontent.com/Medivh-C/SwitchHosts/master/screenshots/cloud_test1.png" alt="Capture" width="960"> 
