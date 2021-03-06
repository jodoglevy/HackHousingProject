# Zillow Personal Advisor

Team name: Aliens vs Predator vs. Brown vs. Board of Education

## Intro

The purpose of Zillow Personal Advisor is to provide Zillow users with a more personalized experience during their home search.

This application was developed February 6-8th, 2015 for the Hack Housing Zillow Hackathon.

Our app is live at https://chrome.google.com/webstore/detail/zillow-personal-advisor/ggkbabbeajcoacmcgobollpffemnkkll. Screenshots are here too. To install the app, just click on the "+ Free" button" and then go to Zillow.com. We integrate with the Zillow profile page and map page.

## Challenge and Approach

Zillow Personal Advisor addresses  many pain points for first time and lower income home buyers, such as 
* What houses can I afford based on my finances?
* Do I qualify for any HUD loan assistance programs, and why?
* Where and from who can I get more infomation on these programs?

Our approach for satisfying this challenge was to:

* Build a Chrome browser extension that extends the functionality on Zillow.com to add advice based on the user's specific finances:
    * Integrate with Mint to pull a user's specific financial information 
    * Advice based on their finances:
      * Provide max house cost that can be used to filter houses on map
    * Advice based on their finances and the area they are searching for homes in:
      * Provide federal aid plans for home loans they qualify for, and why
      * Provide contact information of nearby loan assistance agents (to location they are searching for homes) 
    * Advice based on their finances and a specific home they are viewing:
      * Provide recommendations on specific homes

## Team Members

Our team is comprised of:

    * Adam Levine 
    * Joe Levy
    * Mason Meier
    * Stephen Han

## Technologies, APIs, and Datasets Utilized

We made use of:
    * Mint.com - scrape data from Mint site and make use of Mint's internal API to gather other information
    * JavaScript Chrome extension
      * HTTP request transformer to modify Zillow map page canvas to show houses user can afford/hide houses user can't afford
    * Make use of internal Zillow API to get bank interest rate based on loan amount and down payment
    * Active Housing Counseling Agencies API - return counseling agencies nearby and their contact info if user qualifies for HUD loan assistance programs

## Building and Running

    	* Clone the git repository
	* Open Google Chrome
	* Chrome menu: More Tools -> Extensions  
	* Load Unpacked Extension
	* Select file directory "src" of the cloned repository
	* Enable the extension
	* Go to Zillow profile page to integrate with Mint, and Zillow map page

## Screenshots
Mint data integration:
![Mint Integration](https://github.com/jodoglevy/HackHousingProject/blob/master/images/MintIntegration.png)

Mint profile data on Zillow.com:

![Mint Profile Data](https://github.com/jodoglevy/HackHousingProject/blob/master/images/MintProfileData.png)

Nearby Active Housing Counseling Agencies on Zillow.com:
![Nearby Active Housing Counseling Agencies](https://github.com/jodoglevy/HackHousingProject/blob/master/images/NearbyAdvisors.png)

Filter properties by affordability based on personal finance data on Zillow.com:
![Filter by affordability](https://github.com/jodoglevy/HackHousingProject/blob/master/images/FilterByAffordability.png)

House loan estimate based on personal finance data on Zillow.com:
![House Loan Estimate](https://github.com/jodoglevy/HackHousingProject/blob/master/images/HouseLoanEstimate.png)

## License

Our code is licensed under the MIT License. Pull requests will be accepted to this repo, pending review and approval.
