# Let's Recap

![Lets Do This](./04-knowledge.jpg)

___

## On the Drupal Side

___

# Content Types

<div class="image-slide">

![Drupal Content Types](./04-content-types.png)

- Drupal uses Content Types that allow you to store data.
- These could be things like Blog Posts, Articles, Pages, or any type of "content" you want on your site.

</div>

___

# Fields

<div class="image-slide">

![Drupal Fields](./04-fields.png)

- You can add fields to these content types
- Fields could be any type of information related to that content
- Examples are images, text, dates, taxonomy terms/categories

</div>

___

# Expose the Data

<div class="image-slide">

![Drupal Fields](./04-jsonapi.png)

- We expose the data by turning on the *JSON:API* module
- <cite>that's it</cite>

___

## On the Gatsby Side

Start by creating a new Gatsby Project

```
gatsby new my-project
```

___

# Gatsby Drupal Source Plugin

We install the Gatsby Source Drupal plugin

```
npm install --save gatsby-source-drupal
```

___

## In gatsby-config.js

![Gatsby Config](./04-gatsby-config1.png)

___

# GraphQL is the connector between the two

It allows us to pull in data using something that looks like...

___

![GraphQL Example](./04-teaser.png)

___

## Gatsby creates all of the pages in gatsby-node.js

![GraphQL Example](./04-create.png)

___

![GraphQL Example](./04-create2.png)

___

## This maps to a template

This template defines what data you will receive

as well as how to display that data

___

## In the end, it's all React components

This means you can do anything that you normally could do with React.
