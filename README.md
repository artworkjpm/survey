# How to make a survey?

1. Create in survey.js
2. Style it using old style code
3. Create table to receive answers with correct columns
4. Create form in responsys
5. Save to results table
6. Add survey.js code with html styled into a html file inside responsys
7. Link form to use this html previw

**Now you should have a form, html preview, results table. All you need is the link to the form.**

8. Add the form use code to the forms response code. Create your url to the form, eg could be like:
**${form('wifi_form', "CAMPAIGN_NAME=" + CAMPAIGN, "G_MARKET=" + MARKET, "EMAIL_ADDRESS=" + EMAIL_ADDRESS_)}**
9. Add this url to a campaign, test the link, it should open up your form. TEST TEST TEST the form to see you have values and auto reloads after completion. Good luck!
