# More Variables And Printing

**Strings** - Every time you put " (double-quotes) around a piece of text you have been making a string. A string is how you make something that your program might give to a human. You print them, save them to files, send them to web servers, all sorts of things.

Sometimes you want to embedded some variable into a string. One way for achieve this is by using specialized format sequences and then putting the variables at the end with a special syntax that tells Ruby, “Hey, this is a format string, put these variables in there.”

```ruby
my_name = 'Zed A. Shaw'
my_age = 35
my_height = 74 # inches
my_weight = 180 # lbs
my_eyes = 'Blue'
my_teeth = 'White'
my_hair = 'Brown'
puts "Let's talk about %s." % my_name
puts "He's %d inches tall." % my_height
puts "He's %d pounds heavy." % my_weight
puts "Actually that's not too heavy."
puts "He's got %s eyes and %s hair." % [my_eyes, my_hair]
puts "His teeth are usually %s depending on the coffee." % my_teeth
puts "If I add %d, %d, and %d I get %d." % [my_age, my_height, my_weight, my_age + my_height + my_weight]
```

Type this above into a single ruby file, and from Terminal run:

 `ruby ex5.rb`

---

## **What should you see**

```shell
$ ruby ex5.rb
Let's talk about Zed A. Shaw.
He's 74 inches tall.
He's 180 pounds heavy.
Actually that's not too heavy.
He's got Blue eyes and Brown hair.
His teeth are usually White depending on the coffee. If I add 35, 74, and 180 I get 289.
```

---
---
---

# Todo
* Change all the variables so there isn’t the my_ in front. Make sure you change the name everywhere, not just where you used `=` to set them.
* Try more format sequences.
* Search online for all of the Ruby format sequences.
* Try to write some variables that convert the inches and pounds to centimeters and kilos. Do not just type in the measurements. Work out the math in Ruby.
