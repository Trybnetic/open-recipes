![logo](logo.png)

[![Build Status](https://travis-ci.org/Trybnetic/open-recipes.svg?branch=master)](https://travis-ci.com/Trybnetic/open-recipes)
[![Depfu](https://badges.depfu.com/badges/e601291ebedcf0d3a98d44c90ff31740/overview.svg)](https://depfu.com/github/Trybnetic/open-recipes)
[![License](https://img.shields.io/github/license/Trybnetic/open-recipes.svg)](https://github.com/Trybnetic/open-recipes/blob/master/LICENSE.txt)  



Open Recipes is a simple jekyll theme to organize and host your favorite recipes.  

## Installation
To install Open Recipes you have to install [jekyll](https://jekyllrb.com). After successfully installing jekyll you have to clone this repository to your computer:
```
git clone https://github.com/Trybnetic/open-recipes.git
```
Then switch into the directory and start jekyll:
```
cd open-recipes
bundle exec jekyll serve
```
The last command starts a webserver on your local machine. Now you should have a copy of the site running at `http://127.0.0.1:4000/open-recipes/`. Open this url with your webbrowser and explore the site.  
By changing some of the files (except of the `config.yml`) the changes will be displayed immediately.

## Usage
If you want to add or change recipes you have to navigate to the `_posts` folder. Here you can create one markdown file for each recipe.
If you want to create a new recipe the easiest way is to copy an existing one and change it to your favor.

## Recipe structure
The idea is to create one markdown file per recipe inside the `_posts` folder. A typical file will look like this:
```
---
layout: recipe
title: Super Awesome Recipe
persons: 4
image: superawesomeimage.jpg
---

<!-- ingredients go into the table below -->

| 1 tbsp. | Foo   |
| 200 g   | Bar   |
| 1 pinch | lorem ipsum |
| 2       | eggs |

<!-- ad -->
<!-- do not delete the line above this one -->


<!-- preparation method/steps go below here -->

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
```
The second line of each recipe specifies the layout (in our case it's always `recipe`). In the next line beginning with `title: `, you can specify the title the recipe should have. The next line states the number of persons this recipe serves.  
If you want to show an image alongside your recipe, copy the image to `assets/images/` and put the filename in line 5 after the `image: ` field.
*Images in landscape format with a width of less than 1000px are recommended.*

The ingredients can be put in as a standard markdown table. The preparation steps can be put as free text or as an ordered or unordered list - this is entirely up to you :)

**happy cooking and enjoy your meal!**
