# Let's Recap

![Lets Do This](./04-knowledge.jpg)

___

## On the Drupal Side

___

# Content Types

- Drupal uses Content Types that allow you to store data.
- These could be things like Blog Posts, Articles, Pages, or any type of "content" you want on your site.

___

# Fields

- You can add fields to these content types
- Fields could be any type of information related to that content
- Examples are images, text, dates, taxonomy terms/categories

___

# Expose the Data

We expose the data by turning on the *JSON:API* module

<cite>that's it</cite>

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


```
// In your gatsby-config.js
module.exports = {
  plugins: [
    {
      resolve: `gatsby-source-drupal`,
      options: {
        baseUrl: `https://drupal-local.lndo.site/`,
      },
    },
  ],
}
```

___

# GraphQL is the connector between the two

It allows us to pull in data using something that looks like...

___

```
{
  allArticle {
    edges {
      node {
        title
        internalId
        created(formatString: "DD-MMM-YYYY")
      }
    }
  }
}
```

___

## Gatsby creates all of the pages in gatsby-node.js

Using the CreatePages process (@todo look for code example)

___

## This maps to a template

This template defines what data you will receive

as well a how to display that data

___

## In the end, it's all React components

This means you can do anything that you normally could do with React.



