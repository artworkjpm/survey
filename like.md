LIKEQ1
LIKEQ2
LIKEQ3
DISLIKEQ1
DISLIKEQ2
DISLIKEQ3
WEBVERSION_EMAIL


${form('like_yes', {'usedb':true})}&CAMPAIGN_NAME=${CAMPAIGN?exec}&MODULE_NAME=HERO&MODULE_HEADLINE=${MODULE.HERO_HEADLINE?exec}&MODULE_VARIANT=${MODULE.HERO_VARIANT?exec}&MODULE_BODY_TEXT=${MODULE.HERO_INTRO_TXT?exec}&WEBVERSION_EMAIL=${clickthrough('WEBVERSION')?url('ISO-8859-1')}

${form('like_no', {'usedb':true})}&CAMPAIGN_NAME=${CAMPAIGN?exec}&MODULE_NAME=HERO&MODULE_HEADLINE=${MODULE.HERO_HEADLINE?exec}&MODULE_VARIANT=${MODULE.HERO_VARIANT?exec}&MODULE_BODY_TEXT=${MODULE.HERO_INTRO_TXT?exec}&WEBVERSION_EMAIL=${clickthrough('WEBVERSION')?url('ISO-8859-1')}








//Process to make a survey
Where where the link be used? > newsletters_test/like_dislike_jm

Save html of the form > Survey like with js.htm

Make a form > Survey like jm

Add the form usage code below in newsletter variables

<#assign baseFormUrl ="https://air.norwegian.com/pub/rf">
<#assign formUrl = baseFormUrl + "?_ri_=X0Gzc2X%3DYQpglLjHJlTQGhXYGgzbPGl9Yy0dUtKCzgqYYzdqtMbiW9zaLzc1NwCfVwjpnpgHlpgneHmgJoXX0Gzc2X%3DYQpglLjHJlTQGNIu0CJzfdYgSOhFow3e9E10zdqtMbiW9zaLzc1NwCf">
<#assign formUrl = formUrl + "&RIID_=" + RIID_?c>
<#assign formUrl = formUrl + "&CAMPAIGN_NAME=" + campaign.name>
<#assign formUrl = formUrl + "&EMAIL=" + EMAIL_ADDRESS_>


Create a campaign with links to that will go to the form > like_dislike_jm
In this case the plan is create two campaigns > like_yes, like_no



"${form('like_yes', {'usedb':true})}"
"${form('like_no', {'usedb':true})}"




//Add this to the links

${form('like_yes', {'usedb':true})}&CAMPAIGN_NAME=${CAMPAIGN?exec}&MODULE_NAME=HERO&MODULE_HEADLINE=${MODULE.HERO_HEADLINE?exec}&MODULE_VARIANT=${MODULE.HERO_VARIANT?exec}&WEBVERSION_EMAIL=${clickthrough('WEBVERSION')?url('ISO-8859-1')}




<a href="${formUrl}&Q_LIKE=Y"
<a href="${formUrl}&Q_LIKE=N"


<a href="${form('like_yes', {'usedb':true})}&MODULE_NAME=MODULE&MODULE_HEADLINE=My%20headline">YES</a>

<a href="${form('like_yes', {'usedb':true})}&MODULE_NAME=HERO&MODULE_HEADLINE=${MODULE.HERO_HEADLINE?exec}&MODULE_VARIANT=${MODULE.HERO_VARIANT?exec}"

https://air.norwegian.com/pub/sf/ResponseForm?_ri_=X0Gzc2X%3DYQpglLjHJlTQGtAsl6OFNL8k4zbShtO5wqpoUDq1NNgSzbhcI2iSzf5iEzg4nkSD9HzfnbWiGVXyjLNpLOfhKLX%3DOhmlLjQNHgQNLLgxohluHptQJhuVXMtX%3DYQpglLjHJlTQGlotsErvcRzdcy7k28gf3owhn5zeXzczcAsL8L44iaEKuKPwiK6DaFwcrsT8&_ei_=EolaGGF4SNMvxFF7KucKuWPPEpWxkIYoGtWfcKIMNy3paG22h2bAIWAKI9tpHTXDjHWfqW6IpGdDSR-HFB2Qfxq9r6RMkG6MMkiG3TmpECyupasycM&MODULE_NAME=HERO&MODULE_HEADLINE=Just%20like%20the%20movies

//Make a campaign to place the form html




${}

${clickthrough('WEBVERSION')}

${form(CAMPAIGN, "LANGUAGEID",  "MARKET", "DESTINATION_IATA", "FIRSTNAME", "SURNAME", "EMAIL_ADDRESS_", "REWARD_YN","NL_PROFILE_ID","NL_UNSUB_ID","REWARD_NUMBER","CASHPOINTS","PREFFERED_AIRPORT", "CASHPOINTS_BALANCE")}




If they click no, take them to a form with 4 drop downs
1)	These routes don’t appeal to me
2)	I don’t like the price 
3)	I don’t like the imagery
4)	This content did not inspire me

If they click Yes take them to form:
1)	I like the content
2)	I like the imagery
3)	I like the price
4)	I like receiving these emails











like_dislike_jm

NL market

<#--use ${form('SURVEY_LB_1', {'usedb':true})} as the link url to the survey, it is made in SURVEY_LB_1 campaign in !frameworkSurveys-->

${form('SURVEY_LB_1', {'usedb':true})}

<a href="${form(LIKE_SURVEY, {'usedb':true})}" target="_blank">I like this content</a>

<a href="${form(DISLIKE_SURVEY, {'usedb':true})}" target="_blank">I don't like this content</a>


<a href="${form(campaign.name, {'usedb':true})}" target="_blank">Survey link</a>


<a href="${form(LIKE_SURVEY, {'usedb':true})}" target="_blank">I like this content</a>

<a href="${form(DISLIKE_SURVEY, {'usedb':true})}" target="_blank">I don't like this content</a>

	https://static.cdn.responsys.net/i2/responsysimages/content/nas/icon-positive_20px.png
	https://static.cdn.responsys.net/i2/responsysimages/content/nas/icon-negative_20px.png
