# How to make a survey?

1. Create in survey.js
2. Style it using previous forms styling code and call to Norwegian css file (use wifi form here)
3. Create table to receive answers with correct columns
4. Create form in responsys
5. Save to results table
6. Add survey.js code with html styled into a html file inside responsys
7. Link form to use this html previw

**Now you should have a form, html preview, results table. All you need is the link to the form.**

8. Add the form use criptic code to the forms sendData code. **(function sendDataToResponsys(survey))**
9. Create your url to the form, eg could be like:
**${form('wifi_form', "CAMPAIGN_NAME=" + CAMPAIGN, "G_MARKET=" + MARKET, "EMAIL_ADDRESS=" + EMAIL_ADDRESS_)}**
10. Add this url to a campaign, test the link, it should open up your form. TEST TEST TEST the form to see you have values and auto reloads after completion. Good luck!
