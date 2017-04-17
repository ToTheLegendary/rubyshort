# ruby short syntax
Made ruby simple syntax


#### Map

`user_ids = users.map(&:id)`

#### String and Array:
```
+ String
s= %Q(hello)
s= %q(hello)
+ Array
s= %w(a b c)
s= %W(a b c)
```
#### Random method

`[1,2,3,4,5].sample`

*or*

`[1,2,3,4,5].select(&:even?)`


#### Method always return

```
def get_user_ids(users)
  users.map(&:id)
end
```


#### Multi assignments
```
def values
  [1, 2, 3]
end

one, two, three = values
```


#### Check conditions with '?'

`Framgia.awesome?`

`[].any? # => false`

`1, 2, 3].any? # => true`



#### Unless vs try
* Unless:
  `user.id unless user.nil?`
* Try:
  `user.try(:id)`
  
  

 #### Double Pipe Equals
 `some_variable ||= 10
puts some_variable # => 10`

`some_variable ||= 99
puts some_variable # => 10`

---

  
# ruby short loop

1. FOR LOOP
```
for i in (0..5) do
  puts "#{i}"
end
```


`0..5 == [0, 1, 2, 3, 4, 5]`

2. EACH LOOP
```
(0..5).each do |i|
  puts "#{i}"
end
```

3. BREAK => Kết thúc khối loop
```
(0..5).each do |i|
  break if i == 2
  puts "#{i}"
end
```

4. NEXT => chuyển sang vòng lặp tiếp theo
```
(0..5).each do |i|
  next if i == 2
  puts "#{i}"
end
```


5. WHILE LOOP
```
var1 = 0
while var1 < NUM do
  <!-- this block of code will be executed while conditions are true -->
  puts "#{var1}"
  var1 += 1
end
```

# If for any reason something went wrong, you can always reset the database as follows:

 * Quit the console.
 * Run $ rm -f development.sqlite3 at the command line to remove the database. (We’ll learn a more elegant method for doing this in Chapter 7.)
 * Re-run the migrations using $ rails db:migrate.
 * Restart the console.






