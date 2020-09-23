
# Web Gui Locale

The eyeson default web GUI provided with the [API service](https://www.eyeson.com/developers/)
comes with locale for english (default, en) and german (de). Any additional
language support is community driven. Unfortunately we cannot ensure corectness
and completeness of such, however feel free to create a pull request and
suggest changes or even new languages yourself.

## Usage

Fork the project. Create a new file with the proper locale as name, best start
by copying the default language file `$ cp en.json fr.json`. Translate all
text. Ensure the file is in JSON format, use `$ npm test`. Create a pull
request so we can check your changes and update our application.

```sh
# Choose any locale of: en, de or fr.
$ curl -v -X POST \
  -H "Authorization: <your-api-key>" \
  -d "user[name]=iamgroot" \
  -d "options[custom_fields][locale]=fr" \
  "https://api.eyeson.team/rooms"
```
