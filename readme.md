---
title: Cursor Adapters - Grocery List
type: lab
duration: "1:25"
creator:
    name: Drew Mahrt
    city: NYC
---



# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Cursor Adapters - Grocery List

## Introduction

> ***Note:*** _This can be a pair programming activity or done independently._

In this lab, you will be displaying a list of grocery items from a SQLite database using a `CursorAdapter`. Each grocery item has a name, description, price, and type. On this screen, you will only be showing the name of each item.

## Exercise

#### Requirements

- Extend and complete the SQLiteOpenHelper class to query the database for all of the grocery items
- Make a ListView to display the grocery items
- Use a CursorAdapter to display the queried grocery items

**Bonus:**
- Create a custom layout for the ListView item to show more info from the database

#### Starter code

The `starter-code` folder contains an Android project with the following:

- A MainActivity.java file that prepopulates the database

#### Deliverable

The screenshot below shows what the app should look like.

<p align="center">
  <img src="./screenshots/screen1.png" width="200">
</p>

#### Bonus

- Create a **Detail View** activity for your list
- Your Detail View activity should be called via an Intent in an `OnItemClickListener()`
- Your Detail View should render individual data about each item in your table:
    - ITEM_NAME
    - DESCRIPTION
    - PRICE
    - TYPE

###### Database Table Syntax

```sql
CREATE TABLE SHOPPING_LIST(_id INTEGER PRIMARY KEY AUTOINCREMENT, 
    ITEM_NAME TEXT, 
    DESCRIPTION TEXT, 
    PRICE TEXT, 
    TYPE TEXT);
```

## Additional Resources

- [Cursor](http://developer.android.com/reference/android/database/Cursor.html)
- [CursorAdapter](http://developer.android.com/reference/android/widget/CursorAdapter.html)
- [SimpleCursorAdapter](http://developer.android.com/reference/android/widget/SimpleCursorAdapter.html)


![Creative Commons Non-Commercial License](https://licensebuttons.net/l/by-nc/3.0/88x31.png) Released under the [Creative Commons Non-Commercial License](https://github.com/ga-adi/lab-boilerplate-repository/blob/master/LICENSE)
 
