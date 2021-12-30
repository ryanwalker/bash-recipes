# bash-recipes

### functions
```
add() {
    echo $(($1 + $2));
}
```

### interpolation
```
DEFAULT_USER=$(whoami);
```

### test expressions
```
# man 1 test will show you all of them
[ expression ] 
# or
[[ expression ]]
```



### if/else
```
if [[ $1 == a ]]; then
    echo $(($2 + $3));
elif [[ $1 == s  ]]; then
    echo $(($2 - $3));
elif [[ $1 == m ]]; then
    echo $(($2*$3));
else
    echo "incorrect: $1"
fi
```

### arithmetic
```
number=3;
echo $(($number+2)); # prints 5
```
