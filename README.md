#bash!bin!
echo "enter your birthdate (yyyy.mm.dd):" 
read birthdate 
current_year=$(date | cut -d' ' -f6) 
birth_year=$(echo $birthdate | cut -d'.' -f1) 
age=$((current_year - birth_year)) 
echo "You are $age years old."
