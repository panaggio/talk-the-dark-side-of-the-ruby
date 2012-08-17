!SLIDE transition=scrollUp center

# `String#to_array_of_char`

<!-- TODO: Add cool image -->

!SLIDE

# `String#...`

    @@@ruby
    > 'foo'.to_a
    NoMethodError

    > 'foo'.each_char
     => #<Enumerator: "foo":each_char>

    > 'foo'.chars
     => #<Enumerator: "foo":chars>

!SLIDE

# `String#to_array_of_char`

    @@@ruby
    > 'foo'.chars.to_a
     => ["f", "o", "o"]

    > 'foo'.each_char.to_a
     => ["f", "o", "o"]

    > 'foo'.split(//)
     => ["f", "o", "o"]

    > 'foo'.scan(/./)
     => ["f", "o", "o"]

    # ...
