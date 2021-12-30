# bash-recipes

### functions
```
add() {
    echo $(($1 + $2));
}
```

### command substitution
```
IAM="I am $(whoami)";
IAM="I am `whoami`";
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
### case
```
case $month in

  1)  echo "January"   ;;
  2)  echo "February"  ;;
  3)  echo "March"     ;;
  4)  echo "April"     ;;
  5)  echo "May"       ;;
  6)  echo "June"      ;;
  7)  echo "July"      ;;
  8)  echo "August"    ;;
  9)  echo "September" ;;
  10) echo "October"   ;;
  11) echo "November"  ;;
  12) echo "December"  ;;
  *)
     echo "Error. No month matches: $month"
     echo "Please pass a number between 1 and 12."
     exit 2
     ;;
esac
```
