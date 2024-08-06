# ATM-Mini-Project-
Automated Teller Machines(ATM) allows customers to complete basic transactions without the aid of a branch representative or teller. This project describes the working of ATM. It allows the users to perform certain ... such as check saving balance, deposit funds from the user, withdraw funds from the savings balance account and transfer funds from checking balance to savings balance.

A class ATM is created. It has the following methods:

init(self,acc_bal,check_bal,name,pin): It initializes the values of: self.acc_bal: saving account balance self.check_bal: checking balance self.name: Name of the account holder self.pin: Pin of the ATM card

check_saving_balance(self): It returns the current saving balance

deposit_funds(self): It asks the user to enter the amount to be deposited (funds) and adds it to the saving balance. It also prints the updated saving balance.

withdraw_funds(self): It asks the user to enter the amount to be withdrawn (funds) and checks if the account holds sufficient balance for withdrawal. If the amount is insufficient, it gives warning "Insufficient balance" else subtracts the amount from saving balance. It also prints the updated saving balance.

transfer_funds(self): It asks the user to enter the amount to be withdrawn (amount) from the checking balance and checks if the checking balance is sufficient for withdrawal. If the amount is insufficient, it gives warning "Insufficient balance" else subtracts the amount from checking balance and adds it into saving balance. It also prints the updated saving balance and updated checking balance.

main(self): It is the main function. It asks the user for pin , two times for double authentication. If the pin entered by user is incorrect, it gives the message "Incorrect pin" else, it asks the user for choice 'ch' (1 to 4) and calls the particular methods according to the choice: For ch=1, check_saving_balance(self) is called. For ch=2, deposit_funds(self) is called. For ch=3, withdraw_funds(self) is called. For ch=4, transfer_funds(self) is called. If user enters choice other than 1 to 4, warning is given "Invalid option".

WORKING OF THE PROJECT: User is asked for the following choice(c): c=1 to Register c=2 to Login c=3 to Exit

Register : It is called to generate a pin. In this user is asked for the following details: name:Name
pin: Pin acc_bal: Initial savings balance check_bal: Initial checking balance acc_no: Account number It then adds the details in the dictionary of existing user(d) with account number as the key

Login : It is called to perform the above mentioned actions by the existing users. It asks for the account number(apinn). If the account number is not in the dictionary, it gives the warning "Invalid account number" else creates and object of class ATM and calls the main function.

Exit : It is used to terminate the program.

If user input choice other than 1 to 3, it gives the warning message "Invalid choice".
