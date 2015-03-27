# DealPricingAssignment-jQuery
Interview coding project

NOTE: Sample coding project by Kris Iyer.

Deal Pricing
=====================================================
Background: In the film industry, the “products” that are sold are film rights for a given territory, and date range. For example, a buyer could purchase the exclusive Free-TV rights to distribute Amile in Germany from 2010-2020.

Looking at it more technically, a product is a vector consisting of:

{Film, Right, Territory, Start Date, End Date, License Type}. 

ex:

{Amile, Free-TV, Germany, 2010, 2020, Exclusive}

Task: you have been asked to build a front-end that will allow a Seller to receive an “inquiry” from a Buyer, and respond with pricing. An inquiry consists of a request to purchase several products as explained above.

Assume that the server has already sent you a collection of the products in the inquiry. The service response JSON data has been deserialized into an object. Within any product, a blank StartDate indicates "now", a blank EndDate indicates "perpetuity".

	var inquiry = [
			{
				Title: "Amile",
				TitleId: "50CC799B-F1D6-E311-A5F6-A0B814C922F6",
				Territory: "Germany",
				TerritoryCode: "GER",
				Right: "Free-TV",
				RightCode: "FTV",
				LicenseType: "Exclusive",
				StartDate: "2015",
				EndDate: "2025"
			},
			{
				Title: "Amile",
				TitleId: "50CC799B-F1D6-E311-A5F6-A0B814C922F6",
				Territory: "Germany",
				TerritoryCode: "GER",
				Right: "Pay-TV",
				RightCode: "PTV",
				LicenseType: "Exclusive",
				StartDate: "2015",
				EndDate: "2016"
			},
			{
				Title: "Amile",
				TitleId: "50CC799B-F1D6-E311-A5F6-A0B814C922F6",
				Territory: "Germany",
				TerritoryCode: "GER",
				Right: "Theatrical",
				RightCode: "THR",
				LicenseType: "Exclusive",
				StartDate: "2014",
				EndDate: "2015"
			},
			{
				Title: "The Rock",
				TitleId: "E9BD32D5-86E7-E311-8DAE-B4201D1899F8",
				Territory: "Austria",
				TerritoryCode: "AUS",
				Right: "Free-TV",
				RightCode: "FTV",
				LicenseType: "Non-Exclusive",
				StartDate: "2015",
				EndDate: "2025"
			},
			{
				Title: "The Rock",
				TitleId: "E9BD32D5-86E7-E311-8DAE-B4201D1899F8",
				Territory: "Switzerland",
				TerritoryCode: "SWI",
				Right: "Pay-TV",
				RightCode: "PTV",
				LicenseType: "Exclusive",
				StartDate: "2015",
				EndDate: "2025"
			},
			{
				Title: "Holy Mackerel",
				TitleId: "77843A99-3199-E111-A0E2-180373CF5E18",
				Territory: "Belgium",
				TerritoryCode: "BEL",
				Right: "Theatrical",
				RightCode: "THR",
				LicenseType: "Exclusive",
				StartDate: "",
				EndDate: "" 
			}
		];
		
 
Assignment
-------------------------------------------------------------------------
 

1) Create an HTML mock-up of the pricing UI above. Please note that there are three different views shown – the view should switch in accordance to what is selected in the pricing level dropdown. The interface needs to fulfill the following requirements:

i.	It must display all the products in the inquiry.

ii.	It must have a summary line for every product in the inquiry.

iii.	It must allow the user to select from three pricing "levels": Deal, Title, and Detail 

iv.	It must allow the user to input price(s) based upon the selected pricing level:

a.	Deal level: there is a single flat price for the entire collection of products.

b.	Title level: each group of Titles is priced separately. For example, the three Amile products above would be given a single grouped price.

c.	Detail level: each product is priced individually. 

v.	It must hide (or disable) the non-relevant inputs on the form.

Your mock-up should be styled with CSS, but may use the static data provided in the inquiry  (you can hard-code display values, but the interface should respond appropriately to any user interaction on the screen).
	
 
Evaluation: You will be rated on the following scale:

•	Neatness and Usability of the UI: 40%

•	Technical Ability: 40%

•	Readability of Code: 20%
