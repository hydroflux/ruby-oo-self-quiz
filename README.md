# Quiz: Self

???

## Self Quiz

?: An object is a bundle of code that contains both characteristics and behaviors.

(X) True ( ) False

?: Every object is aware of itself and we can define methods in which we tell objects to operate on themselves.

(X) True ( ) False

?: The `self` keyword refers to the:

( ) The instance of an object ( ) The object that a method is being called on ( ) The class (X) The instance, or object, that the method is being called on

?: What is monkey patching?

( ) The practice of writing Ruby classes from scratch ( ) The practice of overwriting Ruby's core classes (X) The practice of adding methods to or altering Ruby's core classes. ( )  The practice of altering methods in Ruby's core classes.

?:

```ruby
class Car

  attr_accessor :car, :owner

  def initialize(car)
    @car = car
  end

  def honk
    "Beep!"
  end

  def get_title(owner_name)
    self.owner = owner_name
  end

end

lancelot = Car.new("2003 Mitsubishi Lancer")
```

What will `lancelot` return?

( ) nil ( ) 2003 Mitsubishi Lancer (X) An instance of `Car` with `car` defined ( )  An instance of `Car` with `car` and `owner` defined

?: What will `lancelot.get_title("Robert")` return?

(X) Robert ( ) 2003 Mitsubishi Lancer ( ) An instance of `Car` with `car` defined ( )  An instance of `Car` with `car` and `owner` defined

?: After `lancelot.get_title("Robert")` is called, What will `lancelot` return?

( ) Robert ( ) 2003 Mitsubishi Lancer ( ) An instance of `Car` with `car` defined (X)  An instance of `Car` with `car` and `owner` defined

?: You can call any instance methods on `self`.

(X) True ( ) False

???
