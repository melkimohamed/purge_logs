# Role purge logs

#### Features

  - Delete old log files in a specific  folder

#### Requirements
To use this role you should add a specifc folders logs in main.yml with a specific date, example to delete log files in  /var/log/hive only   files old than 30 days, and logs /var/log/knox only  files old than 10 days use this syntax:
```sh
- { name: '/var/log/hive', date: '30d' }
- { name: '/var/log/knox', date: '10d' } 
```
### Inventory
```sh
[hosts]
host1
host2
host3
```

### Example deployement
```sh
ansible-playbook main.yml -i listhosts
```





Author
----

Mohamed Melki
