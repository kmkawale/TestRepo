### Problem Name
Count distinct words in a given paragraph

### Description

You are a data analyst and has been asked to write a program to find out the number of distinct words and their counts for a given input text. The input text is given in the form of a string or a paragraph. The following rules apply to the text
* each word is separated by a space
* distinct words are case insensitive e.g 'It' and 'it' should be reported as 'it' = 2 and not 'It' = 1, 'it' = 1
* new line, tab, space and return characters should not be considered as words
* grammatical characters such as "," and "." should not be part of the word e.g. 'new,' and 'new' should be reported as 'new'= 2 

Write the program using HashMap and the following specifications:

Class:WordCount

* Method:getWordCount
	* Description: Get the count for each distinct word in a given string using HashMap
	* Parameters: String
	* Returns: HashMap
	* Signature: HashMap<String, Int> getWordCount(String inputText)
	* Visibility: public

### Example
	WordCount wcount = new WordCount();
	..
	HashMap<String,Int> hmap = new HashMap(String,Int);
	hmap = wcount.getWordCount(inputText);

### Problem Name
Password change validation

### Description

A bank requires its customers to change their internet banking password based on the following conditions:
* should be atleast 8 characters long
* first digit is not a number
* contains atleast one number
* contains atleast one uppercase and one lowercase alphanumeric character
* contains atleast one character within a set of special chars(!@#$%^&*_+=`~-)
* does not contain space, tab 

Write a program to validate the internet banking password for above conditions.The program should return True if the password is valid else it should return False.

Class: ValidatePassword

* Method: isPasswordValid
  * Description:Checks whether the password matches the required conditions
  * Paramters: String
  * Returns: boolean
  * Signature:boolean isPasswordValid(String password)
  * Visibility: public

### Example
	ValidatePassword vPassword = new ValidatePassword();
	
	if(vPassword.isPasswordValid(password)) //check if password is valid