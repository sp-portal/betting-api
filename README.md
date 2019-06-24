# SP Portal API Client Reference

## **Introduction**
This documentation provides the guide on how to use the API for your sportsbook data needs.

Please contact us if you have any problem.

<br>

### Authentication

#### HTTP Authentication:

API uses HTTP Bearer access authentication. You need to send the Authorization HTTP Request header:

```markdown
Authorization: Bearer <Token>
```

#### Token Based:

To authorize, use this code:

```markdown
curl "api_endpoint_here?token=YOUR-TOKEN"
```

Make sure replace YOUR-TOKEN with your real token.

You will get a **token** from our support. You should pass it as token= in GET query.

<br>

### API Endpoints

API endpoint is started with [https://api.sp-portal.com/](https://api.sp-portal.com)

<br>

### Data Limitation

Data limit is based on the **Plan** you subscribed. 

If you need to know more about our plans, please contact our support.


<br>

### Response

All responses are in JSON and has a success key to indicate it is successful or not.
You'll get **results** if everything moves well, and an (R-Errors) will be thrown if failed.



<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>



<!-- SPORTSBOOK API -->

# **Sportsbook Event API**

## Introduction
Sportsbook API includes Fixtures, Inplay and Results.

<br>

## Inplay Events

<br>

### HTTP Request


**Inplay with Main Market**

GET https://api.sp-portal.com/events/inplaywithmainmarket

```markdown
curl "https://api.sp-portal.com/events/inplaywithmainmarket/SPORT_ID"
```
This will generate list of inplay events with main market and latest odds.

<br>

**Inplay with All Markets**

GET https://api.sp-portal.com/events/inplaywithallmarket

```markdown
curl "https://api.sp-portal.com/events/inplaywithmainmarket/SPORT_ID"
```
This will generate list of inplay events with all markets and latest odds.



<br>

### Query Parameters

Parameter | Required? | Description
--- | --- | --- 
sport_id | No | [Sport Id](#sportid)

`Note there is no pager in this API call. we just return all events.`

<br>

### HTTP Response



<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>


## Upcoming Events

<br>

### HTTP Request

GET https://api.sp-portal.com/events/inplaywithmainmarket

```markdown
curl "https://api.sp-portal.com/events/inplaywithmainmarket/SPORT_ID"
```

This will generate list of upcoming events with main market and odds.

<br>

### Query Parameters

Parameter | Required? | Description
--- | --- | --- 
sport_id | No | [Sport Id](#sportid)

`Note there is no pager in this API call. we just return all events.`

<br>

### HTTP Response



<br><br><br><br><br><br><br><br><br><br>












<br><br><br><br><br><br><br><br><br>
# Glossary

### <a name="sportid"></a>SPORTS ID




















<br><br>


<!-- You can use the [editor on GitHub](https://github.com/isystem20/sp-portal-api/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/isystem20/sp-portal-api/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
 -->