# &#x2600; BLOG APP II

Your blog app should be at the point where the database has been created with columns for title, author, and content. Check that this is the case. Open up the blog_app_api directory, `rails dbconsole`, and `SELECT * FROM blogs`.

&#x1F535; **Activity (35 mins)**

* Create a model for the `posts` table that you made this morning (make the `post.rb` file in the `models` directory, and add the Class with inheritance).

* Generate a migration for making a `Users` table
	* User should have a `name` and `password` (strings)

* Run the migration

* Create a model for `User`

* In `user.rb`, make it so the user `has_many` posts.  

* In `post.rb` make it so a post `belongs_to` a user.

Before we make our seed data, we need the post table to have a foreign key column. The foreign key will reference which user the post belongs to.

* Generate a migration for adding a column to the the `Posts` table. The column should be called `user_id` of type integer.

* Run the migration, and check the `schema.rb`

* Seed your data:

In **Rails console:**

* Create two users
* Create a post for each user
* Check that the relations exist

In **seed.rb**

* Create two more users
* Create three posts, all three posts belong to one of the users
* Run the seed
* Check the data in Rails console and in the database

<br>
<hr>
