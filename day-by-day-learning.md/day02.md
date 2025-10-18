``` #!/bin/bash
# This is for practice.
: << 'comment'
block starts here
anything
written in this
here not be executed


name="Mohan"
echo "Name is $name"
echo "and the date of admission is $(date)"
echo "what is Mohan's friend name?"
read username
echo "You entered $username"

read -p "And his another friend's name: " username
echo "you entered $username"


echo "Here you write your argument number 1: "
read  username  $1
echo "Here you write your argument number 2: "
read username  $2
echo "Here you write your argument number 3: "
read  username  $3
echo "Total number of names as argument here is: $#"
echo "Here are the all of your argument: $@"
comment

read -p "Enter the number: " name
if [[ $name -eq 200 ]]; then
        echo "You are correct!"
elif [[ $name -lt 200 ]]; then
        echo "Your number is less than actual number!"
else
        echo "Your number is greater than actual number!"
fi
```
## for loop
```
#!/bin/bash
# This is for and while loop

for (( num=1 ; num<=5; num++ ))
do
        mkdir "demo$num"
done
```
## while loop
```
#!/bin/bash
: << comment
num=0
while [[ $num -le 5 ]]
do
        echo "lol"
        num = $num+1
done
comment
num=0
while [[ $num -le 10 ]]
do
    echo $num
    num=$((num+2))
done
```
## functoins
```
#!/bin/bash

# Function to greet a user
greet() {
    name=$1
    echo "Hello, $name! Welcome to Bash scripting."
}

# Call the function with a name
#!/bin/bash

# Function to greet a user
greet() {
    name=$1
    echo "Hello, $name! Welcome to Bash scripting."
}

# Call the funct#!/bin/bash

# Function to greet a user
greet() {
    name=$1
    echo "Hello, $name! Welcome to Bash scripting."
}

# Call the function with a name
greet "Yashrajshraj"
greet "Yashraj"
```
