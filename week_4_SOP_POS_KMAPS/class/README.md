# Lab 04 - SOP/POS and KMaps

In this lab, you’ve learned how to apply KMaps, Sum Of Products and Products of
sums to simplify digital logic equations. Then, you’ve proven out that they work
using an implemented design on your Basys3 boards.

## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Lab Summary

I learned how to break down truth tables and implement them into the verilog system for use in circuits.

## Lab Questions

### Why are the groups of 1’s (or 0’s) that we select in the KMap able to go across edges?

KMap  rows and columns only differ by one bit of code. the cells on opposite edges also differ by one bit, so technically they just loop back around.

### Why are the names Sum of Products and Products of Sums?

Each term in an SOP is an AND of literals so it is a product that makes up the 1's and you add those. In a POS each term is an OR of literals or sum and the terms are multiplied together.

### Open the test.v file – how are we able to check that the signals match using XOR?

The test loops through all 16 inputs and XORs the reference output with the minterm and maxterm outputs. Since XOR is 1 only when its inputs differ, a result of 0 means they match, and any 1 triggers a mismatch message and stops the test.

