# How to update Spotlight

Clone git repository https://github.com/texasuka/spotlight 
Install yarn https://classic.yarnpkg.com/en/docs/install/#mac-stable

Run yarn  -- this should install any dependencies for the project

(you also might want to use node.js version 10 -- I suggest using nvm for managing multiple node versions)


src/pages/spotlights has all the spotlight interviews -- look at those files for reference

To create a new spotlight, create a new directory src/pages/spotlights/<new spotlight>
Inside that folder, create index.mdx -- this will be the file that you put the interview stuff in.

Go to src/data/nav-items.yaml and create a new directory & path for the new spotlight.

Test to see if everything looks good with yarn dev 

If everything looks okay, yarn deploy

Update master branch with

git add .
git push origin master

That’s it! Everything should be up at https://spotlight.texasuka.org 


# Gatsby Theme Carbon Starter

## What is this?

> Gatsby [themes](https://www.gatsbyjs.org/docs/themes/) encapsulate all of the
> configuration and implementation details of Gatsby websites. This is a
> starter-kit (boilerplate) with a dependancy on the `gatsby-theme-carbon`
> package. The primary goal of `gatsby-theme-carbon` is to get content authors
> speaking the IBM Design Language with Carbon as soon as possible. It includes
> some sample components/content demos in the `src/pages` directory.

## How do I use it?

Check out our quick
[getting started](https://gatsby-theme-carbon.now.sh/getting-started) guide and
video!

`gatsby-theme-carbon` at it’s core relies on [mdx](https://mdxjs.com/) for page
creation. Check out the `src/pages` directory for some examples for using mdx.

A key feature of Gatsby themes is component shadowing. By simply placing a
component into the `src/gatsby-theme-carbon/components` location, you can
override components used by the theme. You can read more about component
shadowing
[here](https://www.gatsbyjs.org/docs/themes/api-reference#component-shadowing).

You’re also free to make your own components and use them in your MDX pages.

## What’s Next?

[Check out the docs!](https://gatsby-theme-carbon.now.sh)
