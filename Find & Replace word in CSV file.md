```python
import csv
text = open("output.csv", "r")
with open('output.csv','r') as csv_file:
    csv_reader=csv.reader(csv_file)
    for line in csv_reader:
        print(line)
```

    ['Uname; Identifier;First name;Last name']
    ['booker12;9012;Rachel;Booker']
    ['grey;2070;Laura;White']
    ['johnson81;4081;Craig;John']
    ['jenkins46;9346;Mary;Jenkins']
    ['smith79;5079;Jamie;Virat']
    []
    


```python
text = ''.join([i for i in text])
print(text)
```

    Uname; Identifier;First name;Last name
    booker12;9012;Rachel;Booker
    grey;2070;Laura;White
    johnson81;4081;Craig;John
    jenkins46;9346;Mary;Jenkins
    smith79;5079;Jamie;Virat
    
    
    


```python
origin_word=input('Enter the origin word :')
replaced_word=input('Enter the replaced word :')
text = text.replace('{}'.format(origin_word),'{}'.format(replaced_word))  
```

    Enter the origin word :Mary
    Enter the replaced word :Rahul
    


```python
x = open("output.csv","w")
x.writelines(text)
x.close()
```


```python
#save the file
x = open("output.csv","w")
x.writelines(text)
x.close()

#display the output
with open('output.csv','r') as csv_file:
    csv_reader=csv.reader(csv_file)
    for line in csv_reader:
        print(line)
```

    ['Uname; Identifier;First name;Last name']
    ['booker12;9012;Rachel;Booker']
    ['grey;2070;Laura;White']
    ['johnson81;4081;Craig;John']
    ['jenkins46;9346;Rahul;Jenkins']
    ['smith79;5079;Jamie;Virat']
    []
    


```python

```
