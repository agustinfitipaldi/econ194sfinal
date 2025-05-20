# What to do with this repository

In case you have no experience with github, no worries, you don't need to know much (although I'd recommend learning it at one point), just click on the green "<> Code" button in the top-right ish, and in the dropdown select "Download Zip". Then proceed as you usually do with unpacking the zip etc. If you open the bank.qmd file in R studio (after making sure you have all the packages installed using install.packages("packagename")) you should get the html file. You can also just open the html file included

# The Big Idea

The data in the quarto document is a compilation of "Total Asset" and "Total Deposits" as reported in the FDIC through this link https://state-tables.fdic.gov/, by State across time. The main states I think we're interested in are NY and CA, they were the states with the most connection to First Republic and SVB and as you can see they have the most visible effects in the first quarter of 2023.

It's still not clear where precisely we will draw the line for the groups, but I think the effect is rather clear overall. Maybe we just do NY & CA against the rest... so long as we write about our justifications and include decent background we will be fine.

## To-Do

1. Establish groups

2. Calculate means as shown in Lecture slides

3. Do difference in difference thing

4. Make slides

5. Do NBER writeup

### Little To-Do
- add institution type selector
- add date range option
- combine aggregator into scraper
- allow choosing aggregate fields

# Event Overviews

## SVB Overview

1. SVB had purchased a lot of long term treasury bonds

2. To curb inflation there were rate hikes by the fed which decreased the market value of the bonds, leading to significant unrealized losses

3. Rate hikes meant some clients were withdrawing funds to meet liquidity needs

4. With losses and funds being withdrawn SVB started drifting into danger territory (not enough assets to cover liabilities), and word started spreading

5. Social media amongst other things cause lots of individuals to withdraw their money, incurring 42bn in withdrawals on March 9th

6. On March 10th CDFPI seized the bank and put it under the receivership of FDIC

## First Republic

1. In a similar situation to SVB with a high percentage of uninsured deposits, mainly from NY

2. After the March Crisis, Fitch and S&P downgraded FR's credit rating citing these concerns

3. A bunch of banks (JPM, BofA, WF, CITI, and Truist) deposited ~30bn to alleviate concerns

4. Was not enough, and the assets that the bank mainly held were not eligible for some special lending program which had helped SVB

5. On April 28th they began selling assets in order to raise equity, started firing people too.

6. FDIC showed interest in taking over the bank causing stock price to plummet

7. FDIC finally seized FR in after hours trading on the 28th and sold it to JPM on May 1st
