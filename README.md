## Gurka Toolkits
Contains a set of helper kits that can help you for development.

### Install
Open your terminal and type the following command:

```
$ pip install gurka_toolkits
```

### Quick Start
In your Python shell:

```python
>>> from gurka import toolkits
>>>
>>> # Example rupiah formating
>>> money_idn = 45000
>>> toolkits.to_rupiah(money_idn)
'Rp. 45,000.00'
>>>
>>> # Example using autonumber
>>> toolkits.DEFAULT_PREFIX = "PRD" # PRD is a prefix code for product. 
>>> toolkits.DEFAULT_OVERFLOW = 3 # Total digit autonumber
>>> 
>>> toolkits.autonumber()
'PRD001'
>>>
>>> toolkits.autonumber(data=_)
'PRD002'
>>> toolkits.autonumber(data=_)
'PRD003'
>>> toolkits.autonumber(data=_)
'PRD004'
```



