#Xpath Examples:

	/  root
	// any where 

###	Abosolute Xpath (NOT RECOMMENDED)
* Has performance issues, not reliable, can be changed in future (brittle)
* //*[@id=’headsearch’]/div/div[2]/table/tbody/tr/td[2]/input

### Find by TEXT value
* //a[text()='Features']
* //a[contains(text(),'Features']
* //button[contains(text(),'Sign up')]

### Finds button using conditional *AND*
* //button[@type='button' and @class='btn']

### Finds input by attribute using @
* //input[@lightning-input_input='search']

### Find using contains
* //a[contains(text(),'AccountContactRelations/view')]
* //span[contains(text(),'Related Contacts')]
* //a[contains(text(),'/related/AccountContactRelations/view')]


### Starts-with
The following will locate id using substring starts-with:
* id = test-343
* id = test-494
* Example:   //input[starts-with(@id,'test_')]

### Ends-with 
The following will locate id using substring ends-with:
* id = 12230_test-t
* id = 13_test-t
* //input[ends-with(@id,'_test_')]


### How to find number of a particular element on page
```
List <WebElement> linklist = driver.findElements(By.tagName(“a”));
System.out.println(linklist.size)  // print number of anchors <a>

for (int i= 0 ; I < linklist.size; i++ )
{
	String linkText = linklist.get(i).getText();
	System.out.println(linkText)  // print out text of each link.
}
```
