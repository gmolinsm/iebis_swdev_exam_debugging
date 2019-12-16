# Debugging
# First bug
The first bug consists in the '.' being not properly interpreted by the replaceAll() function. This causes the function  
replace all characters by '/'. In order to fix this you can either add '\\' in front of the '.' or simply use the replace()  
function.

# Second bug
The second bug is found in the constructor for StringBuffer, which expects an argument of type String "" but instead receives  
a type char ''.

# Third bug
The switch statement is missing the "break" clauses. This is fixed by doing the following  
```
switch (random.nextInt(2)) {
    case 0:
        word = new StringBuffer("Y");
        break;
    case 1:
        word = new StringBuffer("F");
        break;
    case 2:
        word = new StringBuffer("T");
        break;
}
```

