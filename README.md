#read name from input

read -p "enter user name: " user_name


#code injection:
# while $user_name "1=1 -o x "
# if command will execute the following:
# if [ 1=1 -o x = "denis"] 
#resulting 

#if [ 1=1 -o x = "denis" ]; then

if [ $user_name = "denis" ]; then
    echo "ACCESS GRANTED"
else
echo ACCESS DENIED
fi
------------------------------------------------------------
# to inject and hack this if statement - type in bash terminal "= -o x"
------------------------------------------------------------
