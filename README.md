# kramdown math engine for conversion to MathML

This is a converter for [kramdown](https://kramdown.gettalong.org) that uses
[ritex](https://rubygems.org/gems/ritex/) to convert math formulas to MathML.

Note: Until kramdown version 2.0.0 this math engine was part of the kramdown
distribution.


## Installation

~~~ruby
gem install kramdown-math-ritex
~~~


## Usage

~~~ruby
require 'kramdown'
require 'kramdown-math-ritex'

Kramdown::Document.new(text, math_engine: :ritex).to_html
~~~


## Documentation

To use Ritex, set the option `math_engine` to 'ritex' and make sure that Ritex is available. The
Ritex library can be installed, e.g., via Rubygems by running `gem install ritex`.

> Note that Ritex is released under the GNU GPL version 2 which means that when you use it in
> conjunction with kramdown and your application, your application will automatically also fall
> under the GNU GPL!
>
> If this is a problem for you, consider using the [itex2MML
> math engine](https://github.com/kramdown/math-itex2mml) instead!


## Development

Clone the git repository and you are good to go. You probably want to install
`rake` so that you can use the provided rake tasks.


## License

MIT - see the **COPYING** file.
