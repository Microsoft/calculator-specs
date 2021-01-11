## Financial Calculator

### Feature Pitch Link
https://github.com/Microsoft/calculator/issues/806

### Problem Statement
This will create a new calculation mode, "Financial Worksheets". It will be similar to the date calculator with a combobox at the top to choose modes (modes are tip calculator, compound interest, and mortgage calculator). Target audience: Anyone from financial investors to people going out for lunch.

### Evidence or User Insights
We should do this to offer more tools to calculator users and make this a more feature-packed calculator (GitHub issue: [#806](https://github.com/Microsoft/calculator/issues/806)) and also [Feedback Hub feedback](https://aka.ms/AA9kceq)

### Proposal
Create a new feature "Financial". With it, we can target investors and even students learning about finance. As Windows Calculator from Windows 7 had a few worksheets to calculate mortgage, fuel economy, etc so it will be easier for people transitioning from Win7 to Win10:
<br/>
![Win7Calc](./Assets_and_images/Win7Calc.jpg)
<br/>
The Mortagage Calculator in Windows 7 Calculator

### Goals and Non-Goals
### Goals
* Create a compound interest calculator (Find future value and principle)
* Tips calculator (Find total bill amount, and amount not including tips)
* Mortgage Calculator (Solve for monthly payment and purchase price)

### Non-Goals
* Even more modes

### Success Criteria
Sucess can be mesured with users, and engagement time.

### Feature Requirements
* To find the future value (compound calculator), users can input Principle, term (in day, month or year), times compounded (per year), and interest rate (percentage or decimal) to get the future rate.
> Formula: Future Value = Principle(1+(interest [in decimal]/frequency))^Years* Frequency [[1]](https://www.wikihow.com/Calculate-Compound-Interest#:~:text=Part%202%20of%203%3A%20Calculating%20Compound%20Interest%20on,you%20are%20inputting%20them%20correctly.%20More%20items...%20).

* To find the principle (compound calculator), users can input future value, term (in day, month, or year), times compounded (per year) and interest rate (percentage or decimal)
> Formula: Principle = Future Value / (1+(interest[in decimal]/frequency))^Years* Frequency

* Users can input the bill amout, tip percentage and if they want to split the bill (and if yes, between how many people) and recieve the result.
> Fomula: Total = Amount Due * 1.Tip (percentage) [[2]](https://www.calculatorsoup.com/calculators/financial/tip-calculator.php)

### Feature Details and High-Fidelity Concept

![figure1](./Assets_and_images/Fig1.jpg)
<br/>
Navbar...
<br/>
### Compoound Interest Page

![figure2](./Assets_and_images/Fig2.jpg)
<br/>
Compound interest page, on the calculate future value mode…
<br/>
The result should be the same as long as the the values are equal (just in different time formats, e.g. 365 days equals to 12 months, witch eaquals to 1 year)
<br/>
![figure3](./Assets_and_images/Fig3.jpg)
<br/>
Results (1)...
<br/>
![figure4](./Assets_and_images/Fig4.jpg)
<br/>
Results (2)...
<br/>
![figure5](./Assets_and_images/Fig5.jpg)
<br/>
Results (3)...
<br/>
![figure5](./Assets_and_images/Fig6.jpg)
<br/>
Results (4)...
<br/>
![figure7](./Assets_and_images/Fig7.jpg)
<br/>
If one or more fields are not filled in, an error will show.
<br/>
![figure8](./Assets_and_images/Fig8.jpg)
<br/>
The calculate principle page, if all fields are filled in, the principle field's text does not clear.
<br/>
![gif1](./Assets_and_images/Gif1.gif)
<br/>
Changing modes, as you can see, the principle/future value number box value is filled in automatically.
<br/>
![ReflowFig1](./Assets_and_images/ReflowFig1.jpg)
<br/>
Here's how it will look when minimied to the smallest possible size. All spin buttons will become hidden and grids will tighten. 

### Tip page

![figure7](./Assets_and_images/Fig7.jpg)
<br/>
Tip calculation page, without splitbill on
<br/>
![figure8](./Assets_and_images/Fig8.jpg)
<br/>
Tip calculation page, with splitbill on
<br/>
![figure9](./Assets_and_images/Fig9.jpg)
<br/>
Tip calculation, Results (1)
<br/>
![figure10](./Assets_and_images/Fig10.jpg)
<br/>
Tip calculation, Results (2)
<br/>
![figure11](./Assets_and_images/Fig11.jpg)
<br/>
Tip calculation, Results (3)
<br/>
![figure12](./Assets_and_images/Fig12.jpg)
<br/>
Just like the compound interest calculator, if one or more fields are empty, it will display a warning.

### Appendix
Phases:
Look at devoloping more modes later on.

Risks and Open Issues:
Open issue: I think the everything is up for discussion, including (but not limited to), more modes, rearrange UI, etc. 
Risks: I do not beieve there are any risks.

### References
1. [Wikihow - How to calculate Compound Interest](https://www.wikihow.com/Calculate-Compound-Interest#:~:text=Part%202%20of%203%3A%20Calculating%20Compound%20Interest%20on,you%20are%20inputting%20them%20correctly.%20More%20items...%20)
2. [CalculatorSoup - Tip Calculator](https://www.calculatorsoup.com/calculators/financial/tip-calculator.php)

Note: These are the earliest iterations of the calculator and is _subject to change_. All mocks are from my prototype, which can be found at [chips1234/calculator:FinancialSpec](https://github.com/Chips1234/calculator/tree/FinancialSpec)
