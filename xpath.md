# XPath Examples

## Pathing
/ root
// any node

## Abosolute Path Example - not recommened
//*[@id=’headsearch’]/div/div[2]/table/tbody/tr/td[2]/input<br>

The following is why not to use absolute pathing
  1. performance issues
  2. not reliable
  3. are very brittle, because of the long path, which can easily be changed in the future.<br>
	
## Finds anchor <a> that has **text**
  - //a[text()='Features']

## Finds anchor <a> using **containing certain text** ‘Features’
- //a[contains(text(),'Features']
+ //button[contains(text(),'Sign up')]
