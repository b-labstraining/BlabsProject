# sql-injection Challenge 1

----------------------

Friend, I need your help. Someone is breaking my game.

Someone is exploiting something that causes all entries in our Item Market to be deleted - even those not owned by the person (I know, because some of my listings were deleted). When the entries in the item market are deleted, those items are just gone - I checked, no one possesses those items anymore.

Can you track down what is going on and attempt to duplicate whatever the hacker must be doing, then let me know so I can fix it? After creating a new account and logging in, you should be able to find the Item Market on the Explore page.

Thanks!

-Breakthenet Game Owner

----------------------

Stuck? 
----------------------
<details> 
  <summary>Click for hint 1</summary>
   This is not a black box challenge, you can look in the source code for clues! Specifically, I'd explore [this function](https://github.com/breakthenet/sql-injection-exercises/blob/master/itemmarket.php#L118-L155) - do you see a spot where user input is being put into a query where data is being deleted?
</details>

<details> 
  <summary>Click for hint 2</summary>
  To know more about the database structure, you can review the [sql file](https://github.com/breakthenet/sql-injection-exercises/blob/master/dbdata.sql#L660-L666) in the repo.
</details>

<details> 
  <summary>Click for hint 3</summary>
   The specific query you need to exploit is [here](https://github.com/breakthenet/sql-injection-exercises/blob/master/itemmarket.php#L133). Note that you need to get past the error catching above it, which means you must actually be purchasing a real item that you can afford when attempting to exploit the query.
</details>



