!SLIDE transition=scrollUp center

# Precedência

!SLIDE

# `{}` e `do end`

    @@@ruby
    > puts [1,2].map { |v| v }.join(', ')
     => 1, 2
    > puts [1,2].map do |v| v end.join(', ')
     MethodError: undefined method `join' for nil:NilClass

!SLIDE

# `..` (Range) e `.` (chamada de método)

    @@@ruby
    > 1..5.select { |y| y.odd? }
     NoMethodError: private method `select' called for 5:Fixnum
    > (1..5).select { |y| y.odd? }
     => [1, 3, 5] 

!SLIDE

# (`&&` e `||`) e (`and` e `or`)

    @@@ruby
    > x = true && false; x
     => false
    > x = true and false; x
     => true

    > x = false || true; x
     => true
    > x = false or true; x
     => false
