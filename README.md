## light weight package to verify and get information about Iranian cell phone number
this is a package for checking if input number is a valid iran cell phone number or not
it can give you additional information about its operator and some other useful information like prepaid and postpaid

for now it consist of 3 main method for :

1. verify if input number is real cell phone number
2. determine just operator of cell phone number (if its a wrong phone number returns None)
3. retun type of cell phone based on prepaid or postpaid and its operator 

##### install by pip:
```
pip install iran-mobiles
```

### how to use :
first import module as :
```    
from iran_mobile_va import mobile
```

##### then for validation of a phone number use this method:
```
mobile.is_valid(tel_number)
```
if its valid ,the method returns `True` otherwise returns `False`.

##### for determine just operator of cell phone use this:
```
mobile.tel_operator(tel_number)
```
it returns respective operator but if number is not valid it returns `None`

##### for determine operator and postpaid or prepaid of phone number use this:
```
mobile.tel_information(tel_number)
```
it returns a dictionary that has element of validation and operator of number like `{'validation':'something','operator':'something'}`
but if number is not valid it return `{'validation' = 'False' , 'operator' = 'None'}`



