# Introduction

This package help to convert your excel files (xlsx,xls,csv) to SQL Server database.

# Installation

exceltomysql can be installed as:

Windows:

```python
pip install esceltosqlserver
```

# Dependency

👍   [pandas](https://pandas.pydata.org/)

👍   [pyodbc](https://github.com/mkleehammer/pyodbc)

👍   [sqlalchemy](https://www.sqlalchemy.org/)

# Reslase History

`0.1`

# QuickStart

```python
import exceltosqlserver

# generate the class instance

yourFile  = "test01.xls"  # available for xlsx, xls,csv
yourHostORip  = "localhost"   # you need to change your host if needed, dns: local ip address
yourUsrID = ""
yourPWD   = ""
yourDBname= ""
save2tableName = False  # defsult False

exceltosqlserver(yourFile,yourHoseORip,yourUsrID,yourPWD,yourDBname,save2tableName)


```

```python
output:
Successfully load excel data...
ODBC+Driver+13+for+SQL+Server
Secessfully connected to SQL Server...
Secessfully saved yourtable into SQL Server...
```



# API Reference

exceltosqlserver(`filePath,hostORip=False,usrID =False,pwd=False,database=False,save2tableName`)


filePath: str

hostORip: str  default :False

usrID: str  default: False

pwd: str   default: False

database: str  default:False

save2tableName: str   default:False, will auto save your file name as table name  into mysql database. If assignmed value, will change table name from your file name to the assigned value.
