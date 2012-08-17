!SLIDE transition=scrollUp center

# `require`

!SLIDE

# `require`

    @@@ruby
    # File: ./a.rb
    > require './a'
     => true
    > require './a.rb'
     => false

!SLIDE

# `require`

    @@@ruby
    # File: ./b.strange_extension
    > require './b'
    LoadError: cannot load such file -- b
    > require './b.strange_extension'
    LoadError: cannot load such file -- b.strange_extension

<!-- TODO: Add image about "A cor da grama muda e o burro morre de fome." -->
