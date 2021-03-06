# Joke API

An API for jokes!  This API is primarily for getting a random joke from a growing list of jokes hosted here.  The API uses Azure functions.  Got funny jokes?  See how to submit your jokes down below!

## API Endpoints

### Get a random joke

[https://joke-api.azurewebsites.net/api/joke/](https://joke-api.azurewebsites.net/api/joke/)

returns

```javascript
{
  "id": 56,
  "type": "programming",
  "setup": "There are 10 types of people in this world...",
  "punchline": "Those who understand binary and those who don't"
}
```

### Get a random joke of a specific type

<https://joke-api.azurewebsites.net/api/joke/?joketype=programming>
types of jokes: general, programming, knock-knock (feel free to add jokes outside of these types)

## Contributing a joke

Submit a Pull Request, with your joke added to the jokes/index.json file. Be sure to use this format when adding your joke:

```javascript
{
  "id": <one higher than the previous joke>,
  "type": "your joke's type",
  "setup": "your joke's setup line",
  "punchline": "your joke's punchline"
}
```

### Saying hello

As a super simple example, this function simple appends returns `Hello + name`.

<https://joke-api.azurewebsites.net/api/sayhi/?name=Alex>

returns

```text
Hello Alex
```

## Built With

* [Azure functions](https://docs.microsoft.com/en-us/azure/azure-functions/) - Cloud service, highly recommended
* [Node.js](https://nodejs.org/en/docs/) - Serverside scripting (in Azure)

## Installing

coming soon

## Acknowledgments

* Inspired by [this repository](https://github.com/15Dkatz/official_joke_api).
* jokes gathered from all around the web

## License

This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/alexweininger/joke-api/blob/master/LICENSE) file for details
