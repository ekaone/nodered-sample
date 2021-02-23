```
[
  {
    "id": "39825fb0.4180c",
    "type": "tab",
    "label": "Flow 1",
    "disabled": false,
    "info": ""
  },
  {
    "id": "3d6347d6.186578",
    "type": "http request",
    "z": "39825fb0.4180c",
    "name": "",
    "method": "GET",
    "ret": "txt",
    "paytoqs": "ignore",
    "url": "https://jsonplaceholder.typicode.com/users",
    "tls": "",
    "persist": false,
    "proxy": "",
    "authType": "",
    "x": 370,
    "y": 80,
    "wires": [["c354e1d6.4d5f1"]]
  },
  {
    "id": "36d93d4a.650402",
    "type": "debug",
    "z": "39825fb0.4180c",
    "name": "",
    "active": true,
    "tosidebar": true,
    "console": false,
    "tostatus": false,
    "complete": "false",
    "statusVal": "",
    "statusType": "auto",
    "x": 650,
    "y": 80,
    "wires": []
  },
  {
    "id": "c354e1d6.4d5f1",
    "type": "json",
    "z": "39825fb0.4180c",
    "name": "",
    "property": "payload",
    "action": "",
    "pretty": false,
    "x": 510,
    "y": 80,
    "wires": [["36d93d4a.650402"]]
  },
  {
    "id": "722e46e.c0453b8",
    "type": "inject",
    "z": "39825fb0.4180c",
    "name": "",
    "props": [{ "p": "payload" }, { "p": "topic", "vt": "str" }],
    "repeat": "",
    "crontab": "",
    "once": false,
    "onceDelay": 0.1,
    "topic": "",
    "payload": "true",
    "payloadType": "bool",
    "x": 210,
    "y": 80,
    "wires": [["3d6347d6.186578"]]
  }
]
```
