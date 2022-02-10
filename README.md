<!-- Output copied to clipboard! -->

<!-----

Yay, no errors, warnings, or alerts!

Conversion time: 0.977 seconds.


Using this Markdown file:

1. Paste this output into your source file.
2. See the notes and action items below regarding this conversion run.
3. Check the rendered output (headings, lists, code blocks, tables) for proper
   formatting and use a linkchecker before you publish this page.

Conversion notes:

* Docs to Markdown version 1.0β33
* Wed Feb 09 2022 18:48:23 GMT-0800 (PST)
* Source doc: SENG 438 Assignment 1 Report
* Tables are currently converted to HTML tables.
----->


**SENG 438 Assignment 2 Report	**

**Group: (number)**


<table>
  <tr>
   <td>
    Sr.
   </td>
   <td>
    Name
   </td>
   <td>
    UCID
   </td>
  </tr>
  <tr>
   <td>
    1.
   </td>
   <td>
    Ali Siddiqi
   </td>
   <td>
    30092156
   </td>
  </tr>
  <tr>
   <td>
    2.
   </td>
   <td>
    Jay Gurjar
   </td>
   <td>
    30096042
   </td>
  </tr>
  <tr>
   <td>
    3.
   </td>
   <td>
    Kai Wang
   </td>
   <td>
    30002810
   </td>
  </tr>
  <tr>
   <td>
    4.
   </td>
   <td>
    Mohamed Numan
   </td>
   <td>
    30086940
   </td>
  </tr>
</table>


**<span style="text-decoration:underline;">SENG 438 GROUP</span>**

**Detailed Description of testing strategy**

The testing approach chosen by our group was the black-box test case design technique. Black box testing essentially means testing the code without knowing how the code is written. Test cases in Range are listed below and the chosen range was 0 and 1: 



1. contains():
    1. containsShouldNotBeNan(): The method should return false as the range is a valid range with both arguments as numbers.
    2. containsShouldNotBeNegativeOne(): should return false as the range doesn’t include negative one. 
    3. containsshouldShouldBeZeroPointFive(): should return true as 0.5 is in between 0 and 1. \

2. constrain():
    4. constrainShouldBeZeroPointFive(): should return 0.5 as 0.5 is the mid value between 0 and 1
    5. constrainShouldBeOne() : Should return 1 as one 1 is closest to Postive infinity.
    6. constrainShouldBeNan(): should return Nan as Nan is passed as an argument. \

3. intersects():
    7. intersectShouldNotBeInBetweenNegativeTwoAndNegativeOne(): should return false as exampleRange does not contain the given arguments.
    8.  intersectsShouldNotBeInBetweenOneAndOnePointOne (): should return false as exampleRange does not contain the given arguments.
    9. intersectsShouldBeInBetweenZeroPointFiveAndZeroPointSix(): should return true as example range contains the given points. \

4. combine():
    10. combineShouldBeNull(): should return null as the null to null range is null
    11. combineShouldBeEqualTor1(): should return null as the null to null range is null
    12. combineTestCase(): should be true since the range is still NaN \

5. isNanRange():
    13. isNaNRangeShouldBeTrue(): should return true as Double.NaN is in the NaN range
    14. isNaNRangeShouldBeFalse(): should return false as 1.0 and 2.0 range is not in the NaN range
    15. isNaNRangeShouldBeInNaNRange(): should return false as 2.0 and Double.NaN range is not in the NaN range

We tried testing boundary conditions without knowing how the code was written to find a case where the code crashes. We passed in NaNs and infinities but the code was really well written and Range did not produce any failed unit tests. 

DataUtilities Class Methods tested (20 total test cases)

For the DataUtilities method, we created a total of 20 test cases, 18 which passed and 2 failures. The 2 failed unit tests were testing against illegal arguments and were handled with illegal argument exceptions.



1. createNumberArray(double[ ]): Number[ ]
    1. createNumberArrayWrongType(): Throws an exception for null values
    2. NumberArrayTestBoundary(): Used to test edge values, i.e -1e10 ti 1e10.
2. createNumberArray2D(double[ ] [ ] data): Number[ ][ ]
    3. createNumberArray2DTest(): Used to validate 2D array creation
    4. createNumberArray2DTestSmall(): Used to validate 2D 1x1 array 
    5. createNumberArray2DTestNull(): Used to validate null/empty 2D array
    6. createNumberArray2DTestBoundary(): Used to test edge values, i.e -1e10 to 1e10.
3. calculateColumnTotal(Values2D, int):double
    7. calculateColumnTotalnegBoundary(): Used to test negative boundaries
    8. calculateColumnTotalposBoundary(): Used to test positive boundaries
    9. calculateColumnTotalInvalidIndex(): checks for invalid column index, fail
    10. calculateColumnTotalBlank(): Checks for empty columns
4. calculateRowTotal(Values2D, int):double
    11. calculateRowTotalBlank() : Checks for empty rows
    12. calculateRowTotalInvalidIndex(): Validates invadid row indices, fail
    13. calculateRowTotalposBoundary(): Used to test positive boundaries	
    14. calculateRowTotalnegBoundary(): Used to test negative boundaries
5. Clone
    15. cloneTestEmpty(); Validate an empty clone
    16. cloneTest(); Validate a cloning function
    17. cloneTestNull: Test null inputs
6. Equal
    18. EqualCheckTest
    19. EqualCheckPopulatedTest
    20. EqualCheckNotPopulatedTest

**Discussion TeamWork and Lessons Learned**

We decided that half of us would be on the Range and the other half on Data. Utilities. Each pair of teams completed the 15 test cases for each category. Each team later checked on each other to ensure the test cases were satisfactory and we also asked each other questions throughout the process. We learned that dividing group work into teams and checking on each other works really well for us and allows us to complete the assignments easily and quickly. 

**Difficulties Encountered **

We had lots of trouble following the instructions for setting up the project since the instructions were not clear. Also, we were not sure what naming conventions we should follow and the naming got to be a little weird for some test cases. Also finding boundary test cases for some Range test cases was difficult especially since we did not know how the code was written. Finally, we also had difficulty running the Data. Utility test cases were provided by the professor and got errors when we initially ran them. Eventually, we found out what was wrong with the file and fixed it.

**Comments/Feedback**

In the lab, we got the chance to learn more about test cases and how it's important to write good names for test cases especially. Next time the lab instructions should be more clear. Also, lab instructions should be more clear and not confusing. 

