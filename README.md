# applications-of-category-theory-to-programming-languages

Presentation and supporting code examples given at the Graduate Mathematics Seminar, Cal State Channel Islands, 2018-03-05.

_Please [email me](mailto:danielbrice@gmail.com) if the below instructions fall out of date._

**Note to Programmers:** This presentation is not a monad tutorial. This is a graduate-level talk targeted at mathematicians and computer scientists about programming language research. If you are a software practitioner and you'd like an introduction to monads, I suggest taking a structured approach that builds up to the concept incrementally. If you're interested in learning Haskell specifically, take a look at [Haskell Book](http://haskellbook.com/); however, learning Haskell is not the key to understanding monads, just as understanding monads is not the key to learning Haskell. You'll have much more success learning about monads in your Favorite Language™ (they all have monads, these days) first.

**Note to Math Grad Students:** There aren't a lot of academic positions these days, and non-academic employment options in Mathematics relies heavily on your ability to program. This is not bad news, since if you can learn advanced Math, then you are certainly able to learn programming at the required level. The programming language that Mathematics grad students with no prior programming experience will find least bizzare is almost certainly Haskell, and I highly recommend you take a look at [Haskell Book](http://haskellbook.com/). If you have a decent amount of prior programming experience, I recommend going deeper with the tools you already have exposure to, especially if you have friends who use those tools every day and can help you.

## Setup

To build the presentation and build and run the code examples, you need Java, Scala, and Latex distributions installed and configured on your system. You'll also need the command-line tool _Pandoc_.

**Mac (with Homebrew):**

```sh
brew update && brew upgrade
brew cask install java mactex
brew install scala pandoc
```

**Ubuntu:**

```sh
sudo apt-get update && sudo apt-get full-upgrade
sudo apt-get install default-jdk scala texlive-full pandoc
```

## Build Slideshow

From the `latex/` directory, run `./build.sh`. This will generate `presentation.pdf`.

## Build and Run Code Examples

From the `scala/` directory, run `./build.sh`. This will generate a cornucopia of class files.

Once the class files are built, you can run the various code examples by calling `scala` (again, from the `scala/` directory) with the name of the class whose `main` method you'd like to run:

```sh
scala OrdinaryPartiality
scala MonadicPartiality
scala OrdinaryIO
scala MonadicIO
```
