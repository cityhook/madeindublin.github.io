# Made in Dublin

Everything for the site is available to be modified here. Please read the FAQ first on the website.


## How to add a company

To add your entry, follow [the steps for forking the repo and creating a pull-request][fork repo] and update the `_data/entries.yml` file with your entry's information. The mandatory information to include is:

```
- name: Entry Name
  category: beta | startup | company
  url: www.name.com
  description: Some nice description about the entry. Preferrably between 125-175 characters. Like a long tweet.
```

Optionally, you can add:

```
- ...
  ...
  twitter: entryname
  facebook: entryname
```

Save your entry at the bottom of the file (use spaces for the indentation, not tabs — YAML doesn't like tabs). Note a couple of guidelines (also see the existing entries for a better idea of what to write):

1. **name**: Name of the startup.

2. **category**: Use singular categories (beta instead of betas). Only list each entry as one, otherwise you might break something.

3. **url**: Don't put in the `https://` or `http://`. Preferably, don't put in the `/en` or `/fr` either (if it's a bilingual site) — just link to the root domain since it will likely be the more popular version. Leave off the trailing `/` if your website supports it.

4. **description**: Ease off the *marketing lingo* and definitely leave off the *investor speak* (ie there better not be any appearences of 'digital solution' or 'synergy' anywhere in your description). Use the [third-person narrative](http://en.wikipedia.org/wiki/Third_person) preferrably (ie. don't say 'Shopify is the best platform for YOU to build an online store').

5. **twitter** (optional): leave off the `@`. Preferrably all lowercase.

6. **facebook** (optional): preferrably all lowercase.

**Put the logo in the `_img` directory, not the `img` directory**.

**Commit and push. Then open up a pull-request.**

Lastly, it would be great if you linked to the site somewhere on your own website (ex. a link in your site's footer linking 'Made in Dublin' to this site).

If this all sounds too technical, feel free to [create an issue][create an issue] with the same information (logo, name, description, etc.) and one of the maintainers will add it in when they get time.

## Editing existing entries

Same deal as adding a new entry: [fork and create a pull-request][fork repo]. Only this time half the work is already done for you. Note that changes can be made by anyone, but preference will be given for employees/volunteers of the beta/startup/company.

## Contributing

To setup the environment locally, clone the repo and from the command line:

1. Install [jekyll](https://github.com/jekyll/jekyll) globally with `gem install jekyll`.

If you're only editing the `_data/entries.yml` file, the only command you need is `jekyll serve`, which will build the static site and serve the file at [http://0.0.0.0:3000](http://0.0.0.0:3000).

If you want to do more than just edit the `_data/entries.yml` file, you'll also have to install [Grunt](https://github.com/gruntjs/grunt) and its dependencies:

2. Install [grunt-cli](https://github.com/gruntjs/grunt-cli) globally with `npm install -g grunt-cli`.
3. Navigate to the root `/madeindublin` directory, then run `npm install`. npm will look at [package.json](package.json) and automatically install the necessary local dependencies listed there.

When completed, you'll be able to run the various Grunt commands provided from the command line (look in the GruntFile.js for the additional commands).

**Unfamiliar with `npm`? Don't have node installed?** That's okay. npm stands for [node packaged modules](http://npmjs.org/) and is a way to manage development dependencies through node.js. [Download and install node.js](http://nodejs.org/download/) before proceeding.


## License

Copyright (c) 2014 The Made in Dublin Team

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

### This software is based on Montreal Collective

[Montreal Collective](https://github.com/lukechesser/Montreal-Collective) is licensed under the same terms and is copyright (c) 2013 Luke Chesser. Thank you Luke!

[fork repo]: https://help.github.com/articles/fork-a-repo
[create an issue]: https://github.com/madeindublin/madeindublin.github.io/issues/new

