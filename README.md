# ActiveRecord Lab

## Models
Store model files in `app/models`


Models are Ruby classes that map to database tables in your SQL database (in this case, SQLite). More specifically, they are Ruby classes that inherit from ActiveRecord.

This is a User class in Ruby. It's a plain Ruby class and you could add attributes if you wanted to.
```
class User
    
end
```

This is a User model in Ruby/ActiveRecord (located in `app/models/user.rb` already). Because it inherits from ActiveRecord, it has access to tons of functionality for associating with other models and interacting with the database
```
class User < ActiveRecord::Base
    
end
```

## Topics

- Active Record Migrations
- Active Record Associations
- Class and Instance Methods
- Active Record Querying

## Getting started

**Main commands**
```
bundle install
rake console
rake db:migrate
rake db:seed
```

To get started, run `bundle install` while inside of this directory.

Build out all of the methods listed in the deliverables. The methods are listed
in a suggested order, but you can feel free to tackle the ones you think are
easiest. Be careful: some of the later methods rely on earlier ones.

We've provided you with a tool that you can use to test your code. To use it,
run `rake console` from the command line. This will start a `pry` session with
your classes defined. You can test out the methods that you write here. You are
also encouraged to use the `seeds.rb` file to create sample data to test your
models and associations.

ActiveRecord use the notation `#` for instance methods, and `.` for class
methods. Remember that Active Record give your classes access to a lot of methods already! Keep in mind what methods Active Record gives you access to on each of your
classes when you're approaching the deliverables below.