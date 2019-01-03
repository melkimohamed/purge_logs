# Role purge logs

#### Features

  - Remove logs in a specific folder
  - Remove logs older than a specific date

#### Requirements
To use this role you should add a specifc folders logs in main.yml with a specific date, example to remove logs /var/log/hive only the file old than 30 days, and logs /var/log/knox only the file old than 10 days use this syntax:
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
