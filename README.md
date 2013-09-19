# Ruby on Rails Tutorial: sample application

This is the sample application for
the [*Ruby on Rails Tutorial*](http://railstutorial.org/)
by [Michael Hartl](http://michaelhartl.com/).








#Additional Excersices from Chapter 3:

1.  Make a Contact page for the sample app. Following the model in Listing 3.19, first write a test for the existence of a page at the URL /static_pages/contact by testing for the title “Ruby on Rails Tutorial Sample App | Contact”. Get your test to pass by filling the Contact page with the content from Listing 3.30. (This exercise is solved as part of Section 5.3.)

2.  You may have noticed some repetition in the StaticPages controller spec (Listing 3.19). In particular, the base title, “Ruby on Rails Tutorial Sample App”, is the same for every title test. Using the RSpec let function, which creates a variable corresponding to its argument, verify that the tests in Listing 3.31 still pass. Listing 3.31 introduces string interpolation, which is covered further in Section 4.2.2.

3.  (advanced) As noted on the Heroku page on using sqlite3 for development, it’s a good idea to use the same database in development, test, and production environments to minimize the possibility of subtle incompatibilities. Follow the Heroku instructions for local PostgreSQL installation to install the PostgreSQL database on your local system. Update your Gemfile to eliminate the sqlite3 gem and use the pg gem exclusively, as shown in Listing 3.32. You will also have to learn about the config/database.yml file and how to run PostgreSQL locally. (Note that for security you should add database.yml to your .gitignore file, as shown in Listing 1.7.) Your goal should be to create and configure both the development database and the test database to use PostgreSQL. I especially recommend using Induction to connect to and view the local PostgreSQL database. Warning: You may find this exercise challenging, and I recommend it only for advanced users. If you get stuck, don’t hesitate to skip it; as noted previously, the sample application developed in this tutorial is fully compatible with both SQLite and PostgreSQL.
