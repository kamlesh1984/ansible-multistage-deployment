# ansible-multistage-deployment

Directory-Structure
Inventory
├── roles
│   ├── selinux
│   │   └── tasks
│   │       └── main.yaml
│   └── tomcat
│       ├── files
│       │   └── tomcat-initscript.sh
│       ├── handlers
│       │   └── main.yaml
│       ├── tasks
│       │   └── main.yaml
│       └── templates
│           ├── iptables-save
│           ├── server.xml
│           ├── server.xml.j2_bkp
│           └── tomcat-users.xml
├── site.yaml
├── tomcat-prod
│   ├── group_vars
│   │   ├── tomcat-servers
│   │   └── tomcat-standalone
│   └── hosts
├── tomcat-sit
│   ├── group_vars
│   │   ├── tomcat-servers
│   │   └── tomcat-standalone
│   └── hosts
└── tomcat-uat
    ├── group_vars
    │   ├── tomcat-servers
    │   └── tomcat-standalone
    └── hosts
