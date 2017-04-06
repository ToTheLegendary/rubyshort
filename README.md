# rubyshort
Made ruby simple syntax


#### Map

`user_ids = users.map(&:id)`


---
#### Random method

`[1,2,3,4,5].sample`

*or*

`[1,2,3,4,5].select(&:even?)`

---
#### Method always return

`def get_user_ids(users)
  users.map(&:id)
end`

---
#### Multi assignments
`def values
  [1, 2, 3]
end

one, two, three = values`

---
#### Check conditions with '?'

`Framgia.awesome?`

`[].any? # => false
[1, 2, 3].any? # => true`


---
#### Unless vs try
* Unless:
  `user.id unless user.nil?`
* Try:
  `user.try(:id)`
  
  
 ---
 #### Double Pipe Equals
 `some_variable ||= 10
puts some_variable # => 10`

`some_variable ||= 99
puts some_variable # => 10`

---

  




