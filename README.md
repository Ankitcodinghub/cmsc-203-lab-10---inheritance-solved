# cmsc-203-lab-10---inheritance-solved
**TO GET THIS SOLUTION VISIT:** [CMSC 203 Lab 10 – Inheritance Solved](https://www.ankitcodinghub.com/product/cmsc-203-lab-10-inheritance-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;34584&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CMSC 203 Lab 10 – Inheritance Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<h1>Objectives</h1>
<ul>
<li>Be able to derive a class from an existing class</li>
<li>Be able to define a class hierarchy in which methods are overridden and fields are hidden</li>
<li>Be able to use derived-class objects  Implement a copy constructor</li>
</ul>
<h1>Introduction</h1>
In this lab, you will be creating new classes that are derived from a class called BankAccount. A checking account <strong><em>is a </em></strong>bank account and a savings account <strong><em>is a </em></strong>bank account as well. This sets up a relationship called inheritance, where BankAccount is the superclass and CheckingAccount and SavingsAccount are subclasses. This relationship allows CheckingAccount to inherit attributes from BankAccount (like owner, balance, and accountNumber, but it can have new attributes that are specific to a checking account, like a fee for clearing a check. It also allows CheckingAccount to inherit methods from BankAccount, like deposit, that are universal for all bank accounts. You will write a withdraw method in CheckingAccount that overrides the withdraw method in BankAccount, in order to do something slightly different than the original withdraw method. You will use an instance variable called accountNumber in SavingsAccount to hide the accountNumber variable inherited from BankAccount.

&nbsp;

The UML diagram for the inheritance relationship is as follows:

&nbsp;

&nbsp;

<h1>Task #1 Extending BankAccount</h1>
<ol>
<li>Copy the files AccountDriver.java (code listing 10.1) and BankAccount.java (code listing</li>
</ol>
10.2) from Blackboard. BankAccount.java is complete and will not need to be modified.

<ol start="2">
<li>Create a new class called <strong>CheckingAccount </strong>that <strong>extends BankAccount</strong>. It should contain a static constant <strong>FEE </strong>that represents the cost of clearing one check. Set it equal to 15 cents.</li>
<li>Write a constructor that takes a name and an initial amount as parameters. It should call the constructor for the superclass. It should initialize accountNumber to be the current value in accountNumber concatenated with –10 (All checking accounts at this bank are identified by the extension –10). There can be only one checking account for each account number. Remember since accountNumber is a private member in BankAccount, it must be changed through a mutator method.</li>
<li>Write a new instance method, <strong>withdraw</strong>, that overrides the withdraw method in the superclass. This method should take the amount to withdraw, add to it the fee for check clearing, and call the withdraw method from the superclass. Remember that to override the method, it must have the same method heading. Notice that the withdraw method from the superclass returns true or false depending if it was able to complete the withdrawal or not. The method that overrides it must also return the same true or false that was returned from the call to the withdraw method from the superclass.</li>
<li>Compile and debug this class.</li>
</ol>
<strong>&nbsp;</strong>

<h1>Task #2 Creating a Second Subclass</h1>
<ol>
<li>Create a new class called <strong>SavingsAccount </strong>that <strong>extends BankAccount. </strong>
<ol start="2">
<li>It should contain an instance variable called <strong>rate </strong>that represents the annual interest rate. Set it equal to 2.5%.</li>
<li>It should also have an instance variable called <strong>savingsNumber, </strong>initialized to 0. In this bank, you have one account number, but can have several savings accounts with that same number. Each individual savings account is identified by the number following a dash. For example, 100001-0 is the first savings account you open, 100001-1 would be another savings account that is still part of your same account. This is so that you can keep some funds separate from the others, like a Christmas club account.</li>
<li>An instance variable called <strong>accountNumber </strong>that will hide the accountNumber from the superclass, should also be in this class.</li>
</ol>
</li>
<li>Write a constructor that takes a name and an initial balance as parameters and calls the constructor for the superclass. It should initialize accountNumber to be the current value in the superclass accountNumber (the hidden instance variable) concatenated with a</li>
</ol>
hyphen and then the savingsNumber.

<ol start="3">
<li>Write a method called <strong>postInterest </strong>that has no parameters and returns no value. This method will calculate one month’s worth of interest on the balance and deposit it into the account.</li>
<li>Write a method that overrides the <strong>getAccountNumber </strong>method in the superclass.</li>
<li>Write a copy constructor that creates another savings account for the same person. It should take the original savings account and an initial balance as parameters. It should call the copy constructor of the superclass, assign the savingsNumber to be one more than the savingsNumber of the original savings account. It should assign the accountNumber</li>
</ol>
to be the accountNumber of the superclass concatenated with the hypen and the savingsNumber of the new account.

<ol start="6">
<li>Compile and debug this class.</li>
<li>Use the AccountDriver class to test out your classes. If you named and created your classes and methods correctly, it should not have any difficulties. If you have errors, do not edit the AccountDriver class. You must make your classes work with this program.</li>
<li>Running the program should give the following output:</li>
</ol>
&nbsp;

Account Number 100001-10 belonging to Benjamin Franklin

Initial balance = $1000.00

After deposit of $500.00, balance = $1500.00

After withdrawal of $1000.00, balance = $499.85

Account Number 100002-0 belonging to William Shakespeare

Initial balance = $400.00

After deposit of $500.00, balance = $900.00

Insuffient funds to withdraw $1000.00, balance = $900.00

After monthly interest has been posted, balance = $901.88

Account Number 100002-1 belonging to William Shakespeare

Initial balance = $5.00

After deposit of $500.00, balance = $505.00

Insuffient funds to withdraw $1000.00, balance = $505.00

Account Number 100003-10 belonging to Isaac Newton

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;</strong>

<h1>Code Listing 10.1 (AccountDriver.java)</h1>
<strong>import</strong> java.text.*;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // to use Decimal Format

//Demonstrates the BankAccount and derived classes <strong>public</strong> <strong>class</strong> AccountDriver

{

<strong>public</strong> <strong>static</strong> <strong>void</strong> main(String[] args)

{

<strong>double</strong> put_in = 500;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp; <strong>double</strong> take_out = 1000;

&nbsp;

DecimalFormat myFormat;

String money;

String money_in;&nbsp; &nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; String money_out;

<strong>boolean</strong> completed;

&nbsp;

// to get 2 decimals every time

myFormat = <strong>new</strong> DecimalFormat(“#.00”);

&nbsp;

//to test the Checking Account class&nbsp;&nbsp; CheckingAccount myCheckingAccount =

<strong>new</strong> CheckingAccount (“Benjamin Franklin”, 1000);

System.<strong><em>out</em></strong>.println (“Account Number ”

+ myCheckingAccount.getAccountNumber() +&nbsp;&nbsp;&nbsp; ” belonging to ” + myCheckingAccount.getOwner());&nbsp;&nbsp; money&nbsp; = myFormat.format(myCheckingAccount.getBalance());&nbsp;&nbsp; System.<strong><em>out</em></strong>.println (“Initial balance = $” + money);

myCheckingAccount.deposit (put_in);&nbsp;&nbsp; money_in = myFormat.format(put_in);&nbsp;&nbsp; money&nbsp; = myFormat.format(myCheckingAccount.getBalance());

System.<strong><em>out</em></strong>.println (“After deposit of $” + money_in

+ “,&nbsp; balance = $” + money);

completed = myCheckingAccount.withdraw(take_out);&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; money_out = myFormat.format(take_out);

money&nbsp; = myFormat.format(myCheckingAccount.getBalance());

<strong>if</strong> (completed)

{

System.<strong><em>out</em></strong>.println (“After withdrawal of $” + money_out

+ “,&nbsp; balance = $” + money);

}

<strong>else</strong>

{

System.<strong><em>out</em></strong>.println (“Insuffient funds to withdraw $”

+ money_out + “,&nbsp; balance = $” + money);

}

System.<strong><em>out</em></strong>.println();

&nbsp;

//to test the savings account class&nbsp;&nbsp; SavingsAccount yourAccount =

<strong>new</strong> SavingsAccount (“William Shakespeare”, 400);

System.<strong><em>out</em></strong>.println (“Account Number ”

+ yourAccount.getAccountNumber() +&nbsp;&nbsp;&nbsp;&nbsp; ” belonging to ” + yourAccount.getOwner()); &nbsp;&nbsp;money&nbsp; = myFormat.format(yourAccount.getBalance());&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; System.<strong><em>out</em></strong>.println (“Initial balance = $” + money);

yourAccount.deposit (put_in);&nbsp;&nbsp; money_in = myFormat.format(put_in);&nbsp;&nbsp; money&nbsp; = myFormat.format(yourAccount.getBalance());&nbsp;&nbsp; System.<strong><em>out</em></strong>.println (“After deposit of $” + money_in

+ “,&nbsp; balance = $” + money);

completed = yourAccount.withdraw(take_out);&nbsp;&nbsp; money_out = myFormat.format(take_out);&nbsp;&nbsp; money&nbsp; = myFormat.format(yourAccount.getBalance());

<strong>if</strong> (completed)

{

System.<strong><em>out</em></strong>.println (“After withdrawal of $” + money_out

+ “,&nbsp; balance = $” + money);

}

<strong>else</strong>

{

System.<strong><em>out</em></strong>.println (“Insuffient funds to withdraw $”

+ money_out + “,&nbsp; balance = $” + money);

}

yourAccount.postInterest();

money&nbsp; = myFormat.format(yourAccount.getBalance());&nbsp;&nbsp; System.<strong><em>out</em></strong>.println (“After monthly interest has been posted,”

+ “balance = $” &nbsp;&nbsp;&nbsp; + money);

System.<strong><em>out</em></strong>.println();

&nbsp;

&nbsp;

// to test the copy constructor of the savings account class

SavingsAccount secondAccount =

<strong>new</strong> SavingsAccount (yourAccount,5);

System.<strong><em>out</em></strong>.println (“Account Number ”

+ secondAccount.getAccountNumber()+&nbsp;&nbsp;&nbsp;&nbsp; ” belonging to ” + secondAccount.getOwner());&nbsp;&nbsp; money&nbsp; = myFormat.format(secondAccount.getBalance());&nbsp;&nbsp; System.<strong><em>out</em></strong>.println (“Initial balance = $” + money);

secondAccount.deposit (put_in);&nbsp;&nbsp; money_in = myFormat.format(put_in);&nbsp;&nbsp; money&nbsp; = myFormat.format(secondAccount.getBalance());

System.<strong><em>out</em></strong>.println (“After deposit of $” + money_in

+ “, balance = $” + money);

secondAccount.withdraw(take_out);&nbsp;&nbsp; money_out = myFormat.format(take_out);&nbsp;&nbsp; money&nbsp; = myFormat.format(secondAccount.getBalance());

<strong>if</strong> (completed)

{

System.<strong><em>out</em></strong>.println (“After withdrawal of $” + money_out

+ “,&nbsp; balance = $” + money);

}

<strong>else</strong>

{

System.<strong><em>out</em></strong>.println (“Insuffient funds to withdraw $”

+ money_out + “,&nbsp; balance = $” + money);

}

System.<strong><em>out</em></strong>.println();

&nbsp;

//to test to make sure new accounts are numbered correctly&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp; CheckingAccount yourCheckingAccount =

<strong>new</strong> CheckingAccount (“Issac Newton”, 5000);&nbsp;&nbsp; System.<strong><em>out</em></strong>.println (“Account Number ”

+ yourCheckingAccount.getAccountNumber()

+ ” belonging to ”

+ yourCheckingAccount.getOwner());

&nbsp;

}

}

<h1>Code Listing 10.2 (BankAccount.java)</h1>
/**Defines any type of bank account*/ <strong>public</strong> <strong>abstract</strong> <strong>class</strong> BankAccount

{

/**class variable so that each account has a unique number*/&nbsp; &nbsp;&nbsp;&nbsp; <strong>protected</strong> <strong>static</strong> <strong>int</strong> <em>numberOfAccounts</em> = 100001;

&nbsp;

/**current balance in the account*/&nbsp; &nbsp; <strong>private</strong> <strong>double</strong> balance;&nbsp; &nbsp;&nbsp; /** name on the account*/&nbsp; <strong>private</strong> String owner;

/** number bank uses to identify account*/&nbsp; &nbsp; <strong>private</strong> String accountNumber;

&nbsp;

/**default constructor*/&nbsp; <strong>public</strong> BankAccount()

{

balance = 0;

accountNumber = <em>numberOfAccounts</em> + “”;

<em>numberOfAccounts</em>++;

}

&nbsp;

/**standard constructor

<strong>@param</strong> name the owner of the account &nbsp; <strong>@param</strong> amount the beginning balance*/&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; <strong>public</strong> BankAccount(String name, <strong>double</strong> amount)

{

owner = name;

balance = amount;

accountNumber = <em>numberOfAccounts</em> + “”;

<em>numberOfAccounts</em>++;

}

&nbsp;

/**copy constructor creates another account for the same owner

<strong>@param</strong> oldAccount the account with information to copy &nbsp;&nbsp;&nbsp; <strong>@param</strong> the beginning balance of the new account*/&nbsp; &nbsp; <strong>public</strong> BankAccount(BankAccount oldAccount, <strong>double</strong> amount)

{

owner = oldAccount.owner;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp; balance = amount;

accountNumber = oldAccount.accountNumber;

}

&nbsp;

/**allows you to add money to the account &nbsp;&nbsp;&nbsp; <strong>@param</strong> amount the amount to deposit in the account*/&nbsp; &nbsp;&nbsp; <strong>public</strong> <strong>void</strong> deposit(<strong>double</strong> amount)

{

balance = balance + amount;

}

&nbsp;

/**allows you to remove money from the account if &nbsp; enough money is available,returns true if the transaction was &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; completed, returns false if the there was not enough money. &nbsp;&nbsp;&nbsp; <strong>@param</strong> amount&nbsp; the amount to withdraw from the account &nbsp;&nbsp; <strong>@return</strong> true if there was sufficient funds to complete &nbsp; the transaction, false otherwise*/&nbsp; &nbsp;&nbsp; <strong>public</strong> <strong>boolean</strong> withdraw(<strong>double</strong> amount)

{

<strong>boolean</strong> completed = <strong>true</strong>;

&nbsp;

<strong>if</strong> (amount &lt;= balance)

{

balance = balance – amount;

}

<strong>else</strong>

{

completed = <strong>false</strong>;

}

<strong>return</strong> completed;

}

&nbsp;

/**<u>accessor</u> method to balance &nbsp;&nbsp; <strong>@return</strong> the balance of the account*/

<strong>public</strong> <strong>double</strong> getBalance()

{

<strong>return</strong> balance;

}

&nbsp;

/**<u>accessor</u> method to owner &nbsp;&nbsp;&nbsp;&nbsp; <strong>@return</strong> the owner of the account*/

<strong>public</strong> String getOwner()

{

<strong>return</strong> owner;

}

&nbsp;

/**<u>accessor</u> method to account number &nbsp; <strong>@return</strong> the account number*/

<strong>public</strong> String getAccountNumber()

{

<strong>return</strong> accountNumber;

}

&nbsp;

/**mutator method to change the balance &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>@param</strong> newBalance the new balance for the account*/

<strong>public</strong> <strong>void</strong> setBalance(<strong>double</strong> newBalance)

{

balance = newBalance;

}

&nbsp;

/**mutator method to change the account number &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>@param</strong> newAccountNumber the new account number*/

<strong>public</strong> <strong>void</strong> setAccountNumber(String newAccountNumber)

{

accountNumber = newAccountNumber;

}

}
