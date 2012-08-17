!SLIDE transition=scrollUp center

# underscore

<!-- TODO: Add cool image -->

!SLIDE

# `_`

    @@@ruby
    bad_array = %w[ I d would love to destroy Ruby ]
    foo, _, _, bar, _, _, baz = bad_array
    good_array = [foo, bar, baz].join(' ')

!SLIDE

# `_` & `irb`

    @@@ruby
    > 1
     => 1
    > _
     => 1

    > x, y = _, _+_
     => [1, 2]
    > _
     => [1, 2]

    > (_, _ = _).join(' ')
     => "1 2"

!SLIDE

# `_`

    @@@ruby
    > lambda |_, _| _ }.call(1,2)
     => 1 # 1.9.3
     => 2 # 1.8.7
    > lambda { |x, x| x }.call(1,2)
    SyntaxError: duplicated argument name
